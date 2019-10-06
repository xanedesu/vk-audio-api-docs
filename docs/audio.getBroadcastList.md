## audio.getBroadcastList

Возвращает список друзей и сообществ пользователя, которые транслируют музыку в статус.

> This method can be called with a user token.

### Parameters

<table>
  <tr>
    <td>
      <b>filter</b>
    </td>
    <td>
      определяет, какие типы объектов необходимо получить. Возможные значения:
      <ul>
        <li>
          <i>friends</i> — только друзья; 
        </li>
        <li>
          <i>groups</i> — только сообщества; 
        </li>
        <li>
          <i>all</i> — друзья и сообщества. 
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
      <i>1</i> — будут возвращены только друзья и сообщества, которые транслируют музыку в данный момент. По умолчанию возвращаются все.
      <blockquote>
        flag, either <b>1</b> or <b>0</b>
      </blockquote>
    </td>
  </tr>
</table>

### Result

После успешного выполнения возвращает список объектов [друзей](https://vk.com/dev/objects/user) и [сообществ](https://vk.com/dev/objects/group) с дополнительным полем <b>status_audio</b> — объект [аудиозаписи](https://vk.com/dev/objects/audio), установленной в статус (если аудиозапись транслируется в текущей момент).

### Errors

Global errors can occur while running. See their descriptions on [this page](https://vk.com/dev/errors).