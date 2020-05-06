---
layout: default
---

# リリースノート

<table>
  <thead>
    <tr>
      <th>バージョン</th>
      <th>日付</th>
    </tr>
  </thead>
  <tbody>
    {% for post in site.posts %}
      {% if post.category == 'releases' %}
        <tr>
          <td><a href="{{ post.url }}">{{ post.version }}</a></td>
          <td>{{ post.release_date }}</td>
        </tr>
      {% endif %}
    {% endfor %}
    <tr>
      <td>これより以前のリリースノートはありません</td>
      <td></td>
    </tr>
  </tbody>
</table>


[トップ](/) > [リリースノート](/releases)
