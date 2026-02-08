Conteúdo do curso:
 - https://github.com/lm-academy/github-actions-course

complementos
  - github actions

https://github.com/marketplace?type=actions
https://github.com/aws-actions  

commit convention: 
git add . && git commit -m "feat: training gha: $(date +'%d/%m/%Y %H:%M:%S:%3N')" && git push

https://docs.github.com/pt/actions/reference/workflows-and-actions/workflow-syntax

https://docs.github.com/en/actions/reference/workflows-and-actions/contexts

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