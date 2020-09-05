## audio.search

Returns a list of audio files.

> This method can be called with a [user token](https://vk.com/dev/access_token). [Access rights](https://vk.com/dev/permissions) required: **audio**.

### Parameters

<table>
  <tr>
    <td>
      <b>q</b>
    </td>
    <td>
      Search query string, (e.g. <i>The Beatles</i>)
      <blockquote>
        string
      </blockquote>
    </td>
  </tr>
  <tr>
    <td>
      <b>auto_complete</b>
    </td>
    <td>
      1 — to correct for mistakes in the search query (e.g., if you enter Beetles, the system will search for Beatles)
      <blockquote>
        flag, either <b>1</b> or <b>0</b>
      </blockquote>
    </td>
  </tr>
  <tr>
    <td>
      <b>lyrics</b>
    </td>
    <td>
      1 — to return only audio files that have associated lyrics
      <blockquote>
        flag, either <b>1</b> or <b>0</b>
      </blockquote>
    </td>
  </tr>
  <tr>
    <td>
      <b>performer_only</b>
    </td>
    <td>
      1 — to search only by artist name
      <blockquote>
        flag, either <b>1</b> or <b>0</b>
      </blockquote>
    </td>
  </tr>
  <tr>
    <td>
      <b>sort</b>
    </td>
    <td>
      Sort order:
      <ul>
        <li>
          1 — by duration
        </li>
        <li>
          2 — by popularity
        </li>
        <li>
          0 — by date added
        </li>
      </ul>
      <blockquote>
        int (number)
      </blockquote>
    </td>
  </tr>
  <tr>
    <td>
      <b>search_own</b>
    </td>
    <td>
      <blockquote>
        flag, either <b>1</b> or <b>0</b>
      </blockquote>
    </td>
  </tr>
  <tr>
    <td>
      <b>offset</b>
    </td>
    <td>
      Offset needed to return a specific subset of audio files
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
        positive number, default <b>30</b>, maximum value <b>300</b>
      </blockquote>
    </td>
  </tr>
</table>

### Result

Returns the total results number in **count** field and an array of objects describing [audio](https://vk.com/dev/objects/audio) in <b>items</b> field.

> NOTE: Links to .mp3 files are bound to an IP address.

### Errors

Global errors can occur while running. See their descriptions on [this page](https://vk.com/dev/errors).
