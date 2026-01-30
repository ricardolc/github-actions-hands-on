Doc. again..
instalar complemento github actions...


https://github.com/marketplace?type=actions

https://github.com/aws-actions  

git add . && git commit -m  "continuacao" && git push

https://docs.github.com/pt/actions/reference/workflows-and-actions/workflow-syntax

https://docs.github.com/en/actions/reference/workflows-and-actions/contexts

git add . && git commit -m "feat: training gha: $(date +'%d/%m/%Y %H:%M:%S:%3N')" && git push



Variables

Single Workflow

env:
  NAME: Ricardo (nivel de workflow)

  say-hello:
    runs-on: ubuntu-latest
    env: 
      NAME: Ricardo (nivel de job)
    
    - run: echo "say hello $NAME"
      env: 
        NAME: Ricardo (nivel de step)

Multiple Workflows: 
  - Organization
  - repository
  - environment
      echo ${{ vars.NAME }}