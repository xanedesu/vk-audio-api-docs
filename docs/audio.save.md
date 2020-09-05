## audio.save

Saves audio files after successful [uploading](https://vk.com/dev/upload_files_2?f=8.%20Uploading%20Audio%20Files).

> This method can be called with a [user token](https://vk.com/dev/access_token). [Access rights](https://vk.com/dev/permissions) required: **audio**.

### Parameters

<table>
  <tr>
    <td>
      <b>server</b>
    </td>
    <td>
      This parameter is returned when the audio file is <a href="https://vk.com/dev/upload_files_2?f=8.%20Uploading%20Audio%20Files">uploaded to the server</a>.
      <blockquote>
        int (number), <b>required parameter</b>
      </blockquote>
    </td>
  </tr>
  <tr>
    <td>
      <b>audio</b>
    </td>
    <td>
      This parameter is returned when the audio file is <a href="https://vk.com/dev/upload_files_2?f=8.%20Uploading%20Audio%20Files">uploaded to the server.</a>.
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
      This parameter is returned when the audio file is <a href="https://vk.com/dev/upload_files_2?f=8.%20Uploading%20Audio%20Files">uploaded to the server</a>.
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
      The name of the artist. By default, this is obtained from ID3 tags.
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
      The title of the audio file. By default, this is obtained from ID3 tags.
      <blockquote>
        string
      </blockquote>
    </td>
  </tr>
</table>

### Result

Returns an array of [audio](.) object.

### Errors

<table>
  <tr>
    <td>
      <b>121</b>
    </td>
    <td>
      Invalid hash
    </td>
  </tr>
  <tr>
    <td>
      <b>123</b>
    </td>
    <td>
      Invalid audio
    </td>
  </tr>
  <tr>
    <td>
      <b>270</b>
    </td>
    <td>
      The audio file was removed by the copyright holder and cannot be reuploaded
    </td>
  </tr>
  <tr>
    <td>
      <b>301</b>
    </td>
    <td>
      Invalid filename
    </td>
  </tr>
  <tr>
    <td>
      <b>302</b>
    </td>
    <td>
      Invalid filesize
    </td>
  </tr>
</table>

Global errors can occur while running. See their descriptions on [this page](https://vk.com/dev/errors).
