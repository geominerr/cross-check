#### Ваша оценка - 120 баллов

### Отзыв по пунктам ТЗ:

#### Частично выполненные пункты:

1. The commits are called accordingly to the guideline (https://docs.rs.school/#/git-convention), each commit contains a time-stamp. Time-stamp can be at any language. Accordingly to your time-stamp should be clear, when this commit was done: day of the week, month, day, year, time with seconds (the order can vary) e.g. Commit message example: feat: add basic page layout (Mon, Sep 13, 2021 10:25:24 PM)

   > Отзыв: Коммиты не соответствуют guideline. Screen

2. Icons, meme texts and meme images are exist

   > Отзыв: неправильно указан путь к иконке не отображается... Screen!!!

3. All visual effects when the cursor is hovering over the memes, when the mouse is down on a meme, and when a meme is selected are implemented

   > Отзыв: Нет эффекат при нажатии мема. Screen

4. The entire row (text, icon, and meme image) clickable

   > Отзыв: при клике по мему не выбирается данный элемент

5. Only flexible dimensions are used (rem, em, %, vh, vw, fr and etc.). The accordion is responsive

   > Отзыв: font-size: все в px, можно испольщовать 1rem =16px, или установить 1rem =10px для простоты использования.

6. All blocks/parts of the accordion are in base flow of the dom elements. All elements are not positioned with top, left, right, bottom. float is not used. The value of position is only static. Note: usage of display: none is ALLOWED

   > Отзыв: Используется абсолютное позиционирование, z-index
   > Input можно убрать через opacity или на крайний случай display: none; тз не запрещает.

#### Выполненные пункты:

1. Public repository with name "cssBayan" created

2. Branch gh-pages created

3. The "cssBayan" folder has been created in the gh-pages branch. Deploy is available via link, link example: https://${YOUR_GITHUB_NAME}.github.io/cssBayan/cssBayan/index.html

4. There are at least 5 commits in the gh-pages branch with the history of the project development

5. Pull Request from gh-pages branch to main branch is open. Pull Request name is equal to the task name. Description of the Pull Request was done accordingly to the guideline (https://docs.rs.school/#/pull-request-review-process?id=%D0%A2%D1%80%D0%B5%D0%B1%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F-%D0%BA-pull-request-pr). The link to this Pull Request was submitted to the cross check form. This Pull Request was NOT merged

6. The accordion component is centered on the screen, with equal indents on the left and right

7. Placement of the meme, icons and meme text are the same as in provided example gif images

   > Отзыв: при указании относительных размеров для блока иконки, при transform: rotate() получается как то не очень... ниже скрины

   > ![Screenshot]()

8. Smooth change (transition) of the meme images and icons is done

9. Responsive design with three breakpoints for mobile, tablet, and desktop exist. Accordion is displayed correctly at mobile 320x568, tablet 820x1180, desktop 1920x1080. (Note: breakpoints don't have to be 320x568, 820x1180, 1920x1080)

10. Cursor over the memes (hover) effect only exists for devices that can support hover. This means that the touch device (phone, tablet) doesn't have hover effects, and desktop does have hover effects

    > Отзыв: визуально работает все правильно но технически решение не верно, у вас :hover на всех устройствах свыше 825px висит. Если бы в задании не было бы указано размеров устройств, то как определить какое устройство touch, а какое desktop. 12-16" вполне может быть touch-device

    > Необходимо было сделать медиа запрос, который определяет поддерживает ли данное устройство :hover и уже в нем указывать стили для элементов при наведении. А брекпоинтами изменять размеры блоков, типографию, оформление...

    ```CSS
    @media (hover: hover) {
      .accordion-button {
         color: #7a1c61;
      }

      .accordion-button .plus-icon{
         opacity: 0;
      }

      .accordion-container:hover .accordion-button {
         color: #000000;
      }

      .accordion-container:hover .accordion-button .plus-icon {
         opacity: 1;
      }

      .accordion-input:hover ~ .accordion-content {
         max-height: 80vh;
         transition: 3s;
      }

      .accordion-item:hover > .accordion-content {
         max-height: 80vh;
         transition: 3s;
      }

      .accordion-item:hover > .accordion-button .plus-icon {
         transform: rotate(45deg);
         transition: 1s;
      }
    }
    ```

11. The cursor when it is hovering over the rows of the accordion is changing

12. Pseudo-elements are not used (note 1: pseudo-classes are ALLOWED; note 2: pseudo-elements ONLY from FontAwesome are allowed)

13. Initially, the first meme should be expanded

14. Font size is changed at each device (mobile, tablet, desktop)
