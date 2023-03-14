#### Если есть вопросы или не согласны с моей оценкой пишите здесь или в discord. Хорошего дня!

### Отзыв по пунктам ТЗ:

#### Не выполненные/не засчитанные пункты:

1. The "cssBayan" folder has been created in the gh-pages branch. Deploy is available via link, link example: https://${YOUR_GITHUB_NAME}.github.io/cssBayan/cssBayan/index.html

> Отзыв: необходимо было в вашем репозитории (cssBayan) создать директорию(папку) cssBayan, а уже в ней размещать файлы вашего проекта.

2. Pull Request from gh-pages branch to main branch is open. Pull Request name is equal to the task name. Description of the Pull Request was done accordingly to the guideline (https://docs.rs.school/#/pull-request-review-process?id=%D0%A2%D1%80%D0%B5%D0%B1%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F-%D0%BA-pull-request-pr). The link to this Pull Request was submitted to the cross check form. This Pull Request was NOT merged

> Отзыв: отсутствует ветка main, отсутствует Pull request.

3. Cursor over the memes (hover) effect only exists for devices that can support hover. This means that the touch device (phone, tablet) doesn't have hover effects, and desktop does have hover effects

> Отзыв: Необходимо было сделать медиа запрос, который определяет поддеhживает ли данное устройство :hover и уже в нем указывать стили для элементов при наведении.

```css
@media (hover: hover) {
  .container:hover {
    /* you styles */
  }
}
```

4. Only flexible dimensions are used (rem, em, %, vh, vw, fr and etc.). The accordion is responsive

   > ![Screenshot](https://raw.githubusercontent.com/geominerr/cross-check/main/Stage_1/cssBayan/1/Screenshot_sizes_px.png)
   > Отзыв: Используются все размеры...

5. All blocks/parts of the accordion are in base flow of the dom elements. All elements are not positioned with top, left, right, bottom. float is not used. The value of position is only static. Note: usage of display: none is ALLOWED

   > ![Screenshot](https://raw.githubusercontent.com/geominerr/cross-check/main/Stage_1/cssBayan/1/Screenshot_position.png)
   > Отзыв: Используется абсолютное позиционирование.
   > Используется z-index

---

#### Частично выполненные пункты:

1. The commits are called accordingly to the guideline (https://docs.rs.school/#/git-convention), each commit contains a time-stamp. Time-stamp can be at any language. Accordingly to your time-stamp should be clear, when this commit was done: day of the week, month, day, year, time with seconds (the order can vary) e.g. Commit message example: feat: add basic page layout (Mon, Sep 13, 2021 10:25:24 PM)

   > Отзыв: Коммиты не соответсвуют (отсуствуют секунды, формат отображения 24-х часовой вместо 12)

2. Smooth change (transition) of the meme images and icons is done

   > ![Screenshot](https://raw.githubusercontent.com/geominerr/cross-check/main/Stage_1/cssBayan/1/Screenshot_smooth_change.png)
   > Отзыв: Плавное изменение только мемов, иконки без transitions

3. Responsive design with three breakpoints for mobile, tablet, and desktop exist. Accordion is displayed correctly at mobile 320x568, tablet 820x1180, desktop 1920x1080. (Note: breakpoints don't have to be 320x568, 820x1180, 1920x1080)

   > ![Screenshot](https://raw.githubusercontent.com/geominerr/cross-check/main/Stage_1/cssBayan/1/Screenshot_horizontal_scroll.png)
   > Отзыв: На мобильной версии присутствует горизонтальный скролл при открытом втором меме.

4. All visual effects when the cursor is hovering over the memes, when the mouse is down on a meme, and when a meme is selected are implemented|

   > Отзыв: Отсутсвуют эффекты при выборе мема кликом по области мема.

5. The entire row (text, icon, and meme image) clickable

   > Отзыв: Картинка мема не кликабельна

---

#### Выполненные пункты:

1. Public repository with name "cssBayan" created

2. Branch gh-pages created

3. There are at least 5 commits in the gh-pages branch with the history of the project development

4. The accordion component is centered on the screen, with equal indents on the left and right

5. Icons, meme texts and meme images are exist

6. Placement of the meme, icons and meme text are the same as in provided example gif images

7. The cursor when it is hovering over the rows of the accordion is changing

8. Pseudo-elements are not used (note 1: pseudo-classes are ALLOWED; note 2: pseudo-elements ONLY from FontAwesome are allowed)

9. Initially, the first meme should be expanded

10. Font size is changed at each device (mobile, tablet, desktop)
