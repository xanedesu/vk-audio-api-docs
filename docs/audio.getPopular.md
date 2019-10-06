## audio.getPopular

Returns a list of audio files from the "Popular".

> This method can be called with a user token. [Access rights](https://vk.com/dev/permissions) required: **audio**.

### Parameters

<table>
  <tr>
    <td>
      <b>only_eng</b>
    </td>
    <td>
      <i>1</i> — to return only foreign audio files
      <br>
      <i>0</i> — to return all audio files
      <blockquote>
        flag, either <b>1</b> or <b>0</b>
      </blockquote>
    </td>
  </tr>
  <tr>
    <td>
      <b>genre_id</b>
    </td>
    <td>
      Genre ID. See <a href="https://vk.com/dev/objects/audio_genres">the list of audio genres</a>.
      <blockquote>
        positive number
      </blockquote>
    </td>
  </tr>
  <tr>
    <td>
      <b>offset</b>
    </td>
    <td>
      Offset needed to return a specific subset of audio files.
      <blockquote>
        positive number
      </blockquote>
    </td>
  </tr>
  <tr>
    <td>
      <b>count</b>
    </td>
    <td>
      Number of audio files to return.
      <blockquote>
        positive number, maximum value <b>1000</b>, default <b>100</b>
      </blockquote>
    </td>
  </tr>
</table>

### Result

Returns the total results number in **count** field and an array of objects describing [audio](https://vk.com/dev/objects/audio) in <b>items</b> field.

> NOTE: Links to .mp3 files are bound to an IP address.

### Errors

Global errors can occur while running. See their descriptions on [this page](https://vk.com/dev/errors).