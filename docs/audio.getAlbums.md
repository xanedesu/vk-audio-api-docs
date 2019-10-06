## audio.getAlbums

Возвращает список альбомов аудиозаписей пользователя или группы.

> This method can be called with a user token. [Access rights](https://vk.com/dev/permissions) required: **audio**.

### Parameters

<table>
  <tr>
    <td>
      <b>owner_id</b>
    </td>
    <td>
      идентификатор пользователя или сообщества, у которого необходимо получить список альбомов с аудио.
      <blockquote>
        int (number), current user id is used by default
      </blockquote>
    </td>
  </tr>
  <tr>
    <td>
      <b>offset</b>
    </td>
    <td>
      смещение, необходимое для выборки определенного подмножества альбомов.
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
      количество альбомов, которое необходимо вернуть.
      <blockquote>
        положительное число, по умолчанию <b>50</b>, максимальное значение <b>100</b>
      </blockquote>
    </td>
  </tr>
</table>

### Result

После успешного выполнения возвращает объект, содержащий число результатов в поле <b>count</b> и массив объектов, описывающих альбомы, в поле <b>items</b>. 

Каждый из этих объектов содержит следующие поля: 

* **id** — идентификатор альбома;
* **owner_id** — идентификатор владельца альбома;
*  **title** — название альбома.

### Errors

Global errors can occur while running. See their descriptions on [this page](https://vk.com/dev/errors).