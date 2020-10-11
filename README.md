# ds-action-notify

Example use:

```yaml
name: Test Unit

on: [push]
    
jobs:
   test:
      runs-on: ubuntu-latest

      steps:
         -  uses: actions/checkout@v1

         -  uses: devesharp/ds-action-notify@master
            with:
               MESSAGE: 'Action updated'
               URL: ${{ secrets.NOTIFY_URL }}
               TOKEN: ${{ secrets.NOTIFY_TOKEN }}

```
