<br>
<br>
<br>
<table style="width:100%;border:0px;border-spacing:0px;border-collapse:separate;margin-right:auto;margin-left:auto;">
  <tr>
    <td style="padding:2.5%;width:100%;vertical-align:middle">
      <h2>Internship</h2>
      <p>These are my internship experiences.</p>
    </td>
  </tr>
</table>

<table style="width:100%;border:0px;border-spacing:0px;border-collapse:separate;margin-right:auto;margin-left:auto;">

  {% for post in site.posts %}
  {% for cat in post.categories %}
  {% if cat == 'internship' %}
  <tr>
    <td style="padding:2.5%;width:25%;vertical-align:middle;min-width:120px">
      <img src="{{post.image}}" alt="internship image" style="width:auto; height:auto; max-width:100%;" />
    </td>
    <td style="padding:2.5%;width:75%;vertical-align:middle">
      <h3>{{post.title}}</h3>
      <br>
      {{post.role}}
      <br>
      <em>{{post.duration}}</em>
      <br>
      {{post.organization}}
      <p></p>
      {{ post.excerpt }}
    </td>
  </tr>
  {% endif %}
  {% endfor %}
  {% endfor %}
</table>