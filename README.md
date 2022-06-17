1. На локальном репозитории сделать ветки для:
+ Postman - `git branch Postman`
+ Jmeter - `git branch Jmeter`
+ CheckLists - `git branch CheckLists`
+ Bug Reports - `git branch Bug_Reports`
+ SQL - `git branch SQL`
+ Charles - `git branch Charles`
+ Mobile testing - `git branch Mobile_testing`

2. Запушить все ветки на внешний репозиторий - `git push -u origin --all`

4. В ветке Bag Reports сделать текстовый документ со структурой баг репорта - `git checkout Bug_Reports ; cat > bug_report.txt`
    + ID
    + Title
    + Project
    + STR
    + Actual result
    + Expected result
    + Severity
    + Priority
    + Status
    + Attachments
    + Author
`Enter
CTRL+D`
4. Запушить структуру багрепорта на внешний репозиторий - `git add . ; git commit -m "add bug_report.txt" ; git push`
5. Вмержить ветку Bag Reports в Main - `git checkout Main ; git merge Bug_Reports`
6. Запушить main на внешний репозиторий - `git add . ; git commit -m "merge" ; git push`
7. В ветке CheckLists набросать структуру чек листа - `git checkout CheckLists ; cat > checklist.txt`
    + ID
    + Verification
    + Expected result
    + Status
`Enter
CTRL+D`
8. Запушить структуру на внешний репозиторий - `git add . ; git commit -m "add checklist.txt" ; git push`
9. На внешнем репозитории сделать Pull Request ветки CheckLists в main
  + открыть `https://github.com`. Залогиниться
  + выбрать репозиторий нажать на кнопку `Compare & pull request`
  + нажать на кнопку `Create pull request`
  + нажать на `Merge pull request`
  + нажать на `Confirm merge`
10. Синхронизировать Внешнюю и Локальную ветки Main - `git checkout Main ; git pull`
