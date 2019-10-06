## audio.save

Сохраняет аудиозаписи после успешной [загрузки]().

> This method can be called with a user token. [Access rights](https://vk.com/dev/permissions) required: **audio**.

### Parameters

<table>
  <tr>
    <td>
      <b>server</b>
    </td>
    <td>
      параметр, возвращаемый в результате <a href="">загрузки аудиофайла на сервер</a>.
      <blockquote>
        string, <b>required parameter</b>
      </blockquote>
    </td>
  </tr>
  <tr>
    <td>
      <b>audio</b>
    </td>
    <td>
      параметр, возвращаемый в результате <a href="">загрузки аудиофайла на сервер</a>.
      <blockquote>
        string, <b>required parameter</b>
      </blockquote>
    </td>
  </tr>
  <tr>
    <td>
      <b>hash</b>
    </td>
    <td>
      параметр, возвращаемый в результате <a href="">загрузки аудиофайла на сервер</a>.
      <blockquote>
        string
      </blockquote>
    </td>
  </tr>
  <tr>
    <td>
      <b>artist</b>
    </td>
    <td>
      автор композиции. По умолчанию берется из ID3 тегов. 
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
      название композиции. По умолчанию берется из ID3 тегов.
      <blockquote>
        string
      </blockquote>
    </td>
  </tr>
</table>

### Result

Возвращает массив объект загруженной аудиозаписи с полями <b>id, owner_id, artist, title, url</b>.

### Errors

<table>
  <tr>
    <td>
      <b>121</b>
    </td>
    <td>
      Неверный хэш.
    </td>
  </tr>
  <tr>
    <td>
      <b>123</b>
    </td>
    <td>
      Недопустимый формат аудиозаписи.
    </td>
  </tr>
  <tr>
    <td>
      <b>270</b>
    </td>
    <td>
      Аудиозапись была изъята по запросу правообладателя и не может быть загружена.
    </td>
  </tr>
  <tr>
    <td>
      <b>301</b>
    </td>
    <td>
      Недопустимое имя файла.
    </td>
  </tr>
  <tr>
    <td>
      <b>302</b>
    </td>
    <td>
      Недопустимый размер файла.
    </td>
  </tr>
</table>

Global errors can occur while running. See their descriptions on [this page](https://vk.com/dev/errors).