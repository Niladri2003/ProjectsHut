# Выполните следующие действия, чтобы внести свой вклад📈

**Разберитесь в проекте:**

Ознакомьтесь с целями проекта, архитектурой и существующей кодовой базой. Это позволит вам вносить обоснованный вклад, который соответствует целям проекта.

**Выберите задачу/Создайте задачу:**

Создайте задачу или поработайте над существующей проблемой, если вам назначено. Кроме того, если вы находитесь в `GSSOC'23`, пожалуйста, добавьте `"Я в  GSSOC'23"`, чтобы мы могли добавить метку `GSSOC'23` для этой конкретной проблемы/PR.

**Присвойте номер выпуска:**

Присвойте `#ISSUE_NUMBER` в описании запроса на вытягивание.

** Сначала поработайте над назначенной вам проблемой:**

Мы убедительно просим вас уделить приоритетное внимание работе над назначенной вам проблемой в настоящее время. Настоятельно рекомендуется начать с создания проблемы, прежде чем приступать к созданию запроса на вытягивание. Таким образом, вы можете обрисовать в общих чертах проблему или задачу и облегчить более плавный рабочий процесс. Как только проблема будет установлена, перейдите к внесению необходимых изменений, устранению любых ошибок или включению новых функций для эффективного решения выбранной проблемы/задачи.

**Зафиксируйте изменения:**

После того, как вы добились значительного прогресса или завершили свой вклад, зафиксируйте изменения с помощью описательного сообщения о фиксации. Желательно делать частые, небольшие коммитации, чтобы сделать процесс проверки более управляемым. Пожалуйста, проверьте [обычные коммиты](https://www.conventionalcommits.org/en/v1.0.0/)

## НЕ СПАМЬТЕ  !!! ⚠

Если владелец или владелец обнаружит какую-либо пустую проблему или какое-либо неэтичное поведение со стороны определенного лица, это конкретное лицо будет помечено как «СПАМ», и ему будет запрещено вносить какой-либо вклад или участвовать в будущем в этом проекте.

# 😎 Как добавить свои проекты в ProjectsHut

1. Разветвление этого репозитория

![ Разветвление этого репозитория](https://user-images.githubusercontent.com/88102392/226444075-7d7d28b5-8d88-459a-bb82-38a3f64aaf28.png)

2. Нажмите «Перейти к файлу».

![Перейти к файлу](https://user-images.githubusercontent.com/88102392/226444608-12a2abb9-436c-4843-8893-49029cb4c033.png)

3. Добавьте следующий код в конец 'src/DB/projects.json'

```json
{
  "github_username": "YOUR_GITHUB_USERNAME",
  "Social_media": {
    "gitHub": "YOUR_GITHUB_ACCOUNT_LINK",
    "LinkedIn": "YOUR_LINKEDIN_ACCOUNT_LINK",
    "Instagram": "YOUR_INSTAGRAM_ACCOUNT_LINK",
    "YouTube": "YOUR_YOUTUBE_ACCOUNT_LINK",
    "Тwitter": "YOUR_TWITTER_ACCOUNT_LINK"
  },
  "Projects": [
    {
      "link": "PROJECT_LINK",
      "title": "PROJECT_NAME",
      "description": "PROJECT_DESCRIPTION",
      "tech": "[tech1,tech2]"
    },
    {
      "link": "PROJECT_LINK",
      "title": "PROJECT_NAME",
      "description": "PROJECT_DESCRIPTION",
      "tech": "[tech1,tech2]"
    }
  ]
}
```

4. Зафиксируйте все изменения.

- Добавьте такой коммит только для добавления проектовon `data: project addition by [your-githubuser-name] #issue_number`

> ### Кроме того, если вы предпочитаете запускать проект локально, выполните следующие действия:

1. Перейдите в предпочитаемую папку на вашем компьютере и вставьте следующую команду (только одну из них, если у вас нет настройки ssh, используйте команду HTTP)

- HTTP
    `git clone https://github.com/<YOUR-USERNAME>/ProjectsHut.`
- SSH
    `git clone git@github.com:<YOUR-USERNAME>/ProjectsHut.git`

2. Перейдите в папку проекта

```
 cd ProjectsHut
 ```

3. Создайте файл «.env» в корневую папку, скопируйте код из «.env.example» и добавьте свой «GitHub Personal Access Token» в файл «.env».

4. Установка зависимостей

```
pnpm i
```

5. Теперь сделайте вперед и создайте новую ветку и перейдите к ветке

```
git checkout -b fix-issue-<ISSUE-NUMBER>
```

6. Запуск локально

```
pnpm dev
```

7. Убедитесь, что все тестовые примеры пройдены

```
pnpm test
```

8. После этого вы можете отправить эти изменения, для этого следуйте следующей цепочке команд

   - `git status` (показывает измененные файлы)
   - `git add.` (Добавит все файлы в промежуточную область)
   - `git commit -m "feat/docs/fix: :emoji-name: <EXPLAIN-YOUR_CHANGES>"`
   - > Если вы столкнулись с этой ошибкой во время фиксаций
     >
     > ```diff
     > Husky - хук предварительной фиксации завершен с кодом 1 (ошибка)
     > ```
     >
     > использовать эту команду
     >
     > ```diff
     > формате pnpm
     > ```
   - `git Remote Add Upstream https://github.com/priyankarpal/ProjectsHut.git`
   - `git push origin fix-issue-<ISSUE-NUMBER>`

9. После этого перейдите в разветвленный репозиторий GitHub и перейдите в раздел `Pull Request` раздел
. Теперь вы можете увидеть всплывающее окно с надписью **Pull Request**. Нажмите на всплывающее окно, и вы будете перенаправлены на страницу запроса на вытягивание

10. Теперь заполните шаблон формы pull request и дайте необходимое описание.

11. Нажмите **Отправить**

12. Ура! Вы только что сделали свой вклад в этот проект 🎉

13. Подождите, пока ваш запрос на вытягивание будет рассмотрен и объединен.

> ПРИМЕЧАНИЕ: Пожалуйста, обязательно соблюдайте [Нормы поведения](https://github.com/priyankarpal/ProjectsHut/blob/main/CODE_OF_CONDUCT.md) while contributing.

## Полезные ссылки

- [Руководство по разветвлению GitHub](https://docs.github.com/en/get-started/quickstart/fork-a-repo)
- [Руководство по запросам на вытягивание GitHub](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests)
- [Руководство по проблемам с GitHub](https://docs.github.com/en/issues/tracking-your-work-with-issues/about-issues)
- [Кодекс поведения участников соглашения](https://www.contributor-covenant.org/version/2/1/code_of_conduct/)