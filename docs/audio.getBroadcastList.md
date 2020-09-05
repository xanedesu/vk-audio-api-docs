## audio.getBroadcastList

Returns a list of the user's friends and communities that are broadcasting music in their statuses.

> This method can be called with a [user token](https://vk.com/dev/access_token).

### Parameters

<table>
  <tr>
    <td>
      <b>filter</b>
    </td>
    <td>
      Types of objects to return:
      <ul>
        <li>
          <i>friends</i> — only friends
        </li>
        <li>
          <i>groups</i> — only communities
        </li>
        <li>
          <i>all</i> — both friends and communities (default)
        </li>
      </ul>
      <blockquote>
        string, default <b>all</b>
      </blockquote>
    </td>
  </tr>
  <tr>
    <td>
      <b>active</b>
    </td>
    <td>
      <ul>
        <li>
          <i>1</i> — to return only friends and communities that are broadcasting at the moment.
        </li>
        <li>
          <i>0</i> — to return all friends and communities (default).
        </li>
      </ul>
      <blockquote>
        flag, either <b>1</b> or <b>0</b>
      </blockquote>
    </td>
  </tr>
</table>

### Result

Returns a list of [user](http://vk.com/dev/fields) and [community](http://vk.com/dev/fields_groups) objects, each with the following additional field:
* **status_audio** — an [audio](https://vk.com/dev/objects/audio) object, which is set in status.

### Errors

Global errors can occur while running. See their descriptions on [this page](https://vk.com/dev/errors).
