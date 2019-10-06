## audio.delete

Удаляет аудиозапись со страницы пользователя или сообщества.

> This method can be called with a user token. [Access rights](https://vk.com/dev/permissions) required: **audio**.

### Parameters

<table>
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
      <b>owner_id</b>
    </td>
    <td>
      идентификатор владельца аудиозаписи (пользователь или сообщество).
      <blockquote>
        int (number), <b>required parameter</b>
      </blockquote>
    </td>
  </tr>
</table>

### Result

После успешного выполнения возвращает <i>1</i>.

### Errors

Global errors can occur while running. See their descriptions on [this page](https://vk.com/dev/errors).