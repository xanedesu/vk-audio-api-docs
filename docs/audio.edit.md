## audio.edit

Edits an audio file on a user or community page.

> This method can be called with a [user token](https://vk.com/dev/access_token). [Access rights](https://vk.com/dev/permissions) required: **audio**.

### Parameters

<table>
  <tr>
    <td>
      <b>owner_id</b>
    </td>
    <td>
      ID of the user or community that owns the audio file.
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
      Audio file ID.
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
      Name of the artist.
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
      Title of the audio file.
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
      Text of the lyrics of the audio file.
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
      Genre of the audio file. See the list of <a href="https://vk.com/dev/objects/audio_genres">audio genres</a>.
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
      <ul>
        <li>
          <i>1</i> —  audio file will not be available for search
        </li>
        <li>
          <i>0</i> —  audio file will be available for search (default)
        </li>
      </ul>
      <blockquote>
        flag, either <b>1</b> or <b>0</b>
      </blockquote>
    </td>
  </tr>
</table>

### Result

If lyrics were entered by the user, returns **lyrics_id**. Otherwise, returns **0**.

### Errors

Global errors can occur while running. See their descriptions on [this page](https://vk.com/dev/errors).
