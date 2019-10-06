## audio.setBroadcast

description

> This method can be called with a user token. [Access rights](https://vk.com/dev/permissions) required: **audio**.

### Parameters

<table>
  <tr>
    <td>
      <b>audio</b>
    </td>
    <td>
      ID of the audio file to be shown in status (e.g., <i>1_190442705</i>). If the parameter is not set, the audio status of given communities and user will be deleted.
      <blockquote>
        string
      </blockquote>
    </td>
  </tr>
  <tr>
    <td>
      <b>target_ids</b>
    </td>
    <td>
      IDs of communities and user whose statuses will be included in the broadcast. Use a negative value to designate a community ID. By default, current user ID.
      <blockquote>
        list of comma-separated numbers, the maximum number of elements allowed is <b>20</b>
      </blockquote>
    </td>
  </tr>
</table>

### Result

Returns a new setting value.

### Errors

Global errors can occur while running. See their descriptions on [this page](https://vk.com/dev/errors).