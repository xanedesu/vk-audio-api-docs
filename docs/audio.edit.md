## audio.edit

Редактирует данные аудиозаписи на странице пользователя или сообщества.

> This method can be called with a user token. [Access rights](https://vk.com/dev/permissions) required: **audio**.

### Parameters

<table>
  <tr>
    <td>
      <b>owner_id</b>
    </td>
    <td>
      идентификатор владельца аудиозаписи (пользователь или сообщество).
      <blockquote>
        Обратите внимание, идентификатор сообщества в параметре <b>owner_id</b> необходимо указывать со знаком "<b>-</b>" — например, <b>owner_id</b> =<i>-1</i>
        соответствует идентификатору сообщества <a href="https://vk.com/club1">ВКонтакте API</a>
        (club1)
      </blockquote>
      <blockquote>
        int (number), <b>required parameter</b>
      </blockquote>
    </td>
  </tr>
  <tr>
    <td>
      <b>audio_id</b>
    </td>
    <td>
      идентификатор аудиозаписи.
      <blockquote>
        positive number, <b>required parameter</b>
      </blockquote>
    </td>
  </tr>
  <tr>
    <td>
      <b>artist</b>
    </td>
    <td>
      новое название исполнителя.
      <blockquote>
        string
      </blockquote>
    </td>
  </tr>
  <tr>
    <td>
      <b>title</b>
    </td>
    <td>
      новое название композиции.
      <blockquote>
        string
      </blockquote>
    </td>
  </tr>
  <tr>
    <td>
      <b>text</b>
    </td>
    <td>
      новый текст аудиозаписи.
      <blockquote>
        string
      </blockquote>
    </td>
  </tr>
  <tr>
    <td>
      <b>genre_id</b>
    </td>
    <td>
      идентификатор жанра из <a href="https://vk.com/dev/objects/audio_genres">списка аудио жанров</a>.
      <blockquote>
        positive number
      </blockquote>
    </td>
  </tr>
  <tr>
    <td>
      <b>no_search</b>
    </td>
    <td>
      <i>1</i> — аудиозапись не будет доступна в поиске. По умолчанию: <i>0</i>.
      <blockquote>
        flag, either <b>1</b> or <b>0</b>
      </blockquote>
    </td>
  </tr>
</table>

### Result

После успешного выполнения возвращает идентификатор текста, введенного пользователем, если текст не был введен, вернет <i>0</i>.

### Errors

Global errors can occur while running. See their descriptions on [this page](https://vk.com/dev/errors).