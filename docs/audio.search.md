## audio.search

Возвращает список аудиозаписей в соответствии с заданным критерием поиска.

> This method can be called with a user token. [Access rights](https://vk.com/dev/permissions) required: **audio**.

### Parameters

<table>
  <tr>
    <td>
      <b>q</b>
    </td>
    <td>
      текст поискового запроса, например, <i>The Beatles</i>.
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
      Если этот параметр равен <i>1</i>, возможные ошибки в поисковом запросе будут исправлены. Например, при поисковом запросе <i>Иуфедуы</i> поиск будет осуществляться по строке <i>Beatles</i>.
      <blockquote>
        флаг, может принимать значения <b>1</b> или <b>0</b>
      </blockquote>
    </td>
  </tr>
  <tr>
    <td>
      <b>lyrics</b>
    </td>
    <td>
      Если этот параметр равен <i>1</i>, поиск будет производиться только по тем аудиозаписям, которые содержат тексты.
      <blockquote>
        флаг, может принимать значения <b>1</b> или <b>0</b>
      </blockquote>
    </td>
  </tr>
  <tr>
    <td>
      <b>performer_only</b>
    </td>
    <td>
      Если этот параметр равен <i>1</i>, поиск будет осуществляться только по названию исполнителя.
      <blockquote>
        флаг, может принимать значения <b>1</b> или <b>0</b>
      </blockquote>
    </td>
  </tr>
  <tr>
    <td>
      <b>sort</b>
    </td>
    <td>
      Вид сортировки. <i>2</i> — по популярности, <i>1</i> — по длительности аудиозаписи, <i>0</i> — по дате добавления.
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
      — искать по аудиозаписям пользователя, <i>0</i> — не искать по аудиозаписям пользователя. По умолчанию: <i>0</i>.
      <blockquote>
        флаг, может принимать значения <b>1</b> или <b>0</b>
      </blockquote>
    </td>
  </tr>
  <tr>
    <td>
      <b>offset</b>
    </td>
    <td>
      смещение, необходимое для выборки определенного подмножества аудиозаписей. По умолчанию: <i>0</i>.
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
      количество аудиозаписей, информацию о которых необходимо вернуть. 
      <blockquote>
        Обратите внимание — даже при использовании параметра offset для получения информации доступны только первые <b>1000</b> результатов.
      </blockquote>
      <blockquote>
        positive number, maximum value <b>300</b>, default <b>30</b>
      </blockquote>
    </td>
  </tr>
</table>

### Result

Returns the total results number in **count** field and an array of objects describing [audio](https://vk.com/dev/objects/audio) in <b>items</b> field.

> NOTE: Links to .mp3 files are bound to an IP address.

### Errors

Global errors can occur while running. See their descriptions on [this page](https://vk.com/dev/errors).