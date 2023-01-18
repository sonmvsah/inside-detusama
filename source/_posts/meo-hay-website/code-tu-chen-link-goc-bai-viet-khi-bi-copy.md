---
title: Code JavaScript tự chèn link gốc bài viết khi copy
categories: meo-hay-website
tags: [Mẹo hay website, Chống copy nội dung websitge]
---

## Đoạn code javaScript tự dán

- Tự dán cho dân DEV và người chuyên nghiệp
- Chống chỉ định cho người không có thời gian

{% codeblock auto add link lang:javascript https://maivietson.com Nguồn: Mai Việt Sơn %}
<script type="text/javascript">
    function addLink() {
        var body_element = document.getElementsByTagName("body")[0];
        var selection;
        selection = window.getSelection();
        var pagelink =
            "<br/><br/>Link nguồn : <a href='" +
            document.location.href +
            "'>" +
            document.location.href +
            "</a>";
        var copytext = selection + pagelink;
        var newdiv = document.createElement("div");
        newdiv.style.position = "absolute";
        newdiv.style.left = "-99999px";
        body_element.appendChild(newdiv);
        newdiv.innerHTML = copytext;
        selection.selectAllChildren(newdiv);
        window.setTimeout(function() {
            body_element.removeChild(newdiv);
        }, 0);
    }
    document.oncopy = addLink;
</script>
{% endcodeblock %}