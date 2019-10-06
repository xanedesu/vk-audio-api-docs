## audio.getById

Возвращает информацию об аудиозаписях по их идентификаторам.

> This method can be called with a user token. [Access rights](https://vk.com/dev/permissions) required: **audio**.

### Parameters

<table>
  <tr>
    <td>
      <b>audios</b>
    </td>
    <td>
      идентификаторы аудиозаписей, информацию о которых необходимо вернуть, в виде {owner_id}_{audio_id}.
      <blockquote>
        список слов, разделенных через запятую, <b>обязательный параметр</b>
      </blockquote>
    </td>
  </tr>
</table>

### Result

После успешного выполнения возвращает массив объектов [аудиозаписей](https://vk.com/dev/objects/audio).

> NOTE: Links to .mp3 files are bound to an IP address.

### Errors

Global errors can occur while running. See their descriptions on [this page](https://vk.com/dev/errors).