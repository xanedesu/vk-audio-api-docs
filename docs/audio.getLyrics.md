## audio.getLyrics

Returns lyrics associated with an audio file.

> This method can be called with a [user token](https://vk.com/dev/access_token). [Access rights](https://vk.com/dev/permissions) required: **audio**.

### Parameters

<table>
  <tr>
    <td>
      <b>lyrics_id</b>
    </td>
    <td>
      Lyrics ID (could be obtained with <a href="audio.get.html">audio.get</a>, <a href="audio.getById.html">audio.getById</a>, or <a href="audio.search.html">audio.search</a> methods).
      <blockquote>
        int (number), <b>required parameter</b>
      </blockquote>
    </td>
  </tr>
</table>

### Result

Returns a <b>lyrics</b> object containing the following fields:

* **lyrics_id** — Lyrics ID.
* **text** — Lyrics text.

> NOTE: **/n** is used as a line break in the lyrics text.

### Errors

Global errors can occur while running. See their descriptions on [this page](https://vk.com/dev/errors).
