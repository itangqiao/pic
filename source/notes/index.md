---
wiki: notes # 这个跟上面的 /wiki/notes.yml 关联起来
menu_id: notes # 这个跟配置文件中的 `menubar.items.notes` 关联起来，这很重要，如果没有这个，就像普通的wiki项目一样了
leftbar:
  - mark
base_dir: /notes/
tree:
  - mark/index
  - mark/collection
---

{% timeline api:https://memos.casa.itangqiao.top:33333/api/v1/memo?creatorId=1&limit=10 type:memos avatar:/assets/images/avatar2.webp %}
{% endtimeline %}

<!-- {% timeline api:https://api.github.com/repos/itangqiao/mark/issues %}{% endtimeline %} -->