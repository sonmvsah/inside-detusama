---
title: Code JavaScript tự chèn link gốc bài viết khi copy
categories: tips , plugins
tags: [Mẹo hay website, Chống copy nội dung websitge]
thumbnail: /images/posts/tu-dong-chen-link-bai-viet-goc-khi-bi-copy.jpg
---
## Chống Copy nội dung phải đúng cách
Có khá nhiều người lựa chọn cách chống copy nội dung bằng những đoạn mã javascript hoặc css
Tuy nhiên, công dụng đoạn mã lại nhắm vào chặn thao tác của người dùng.
Nếu đó là những thao tác phức tạp và ít người dùng thì không sao, Ngược lại,
thao tác copy và đặc biệt là thao tác click chuột phải được sử dụng liên tục và ở nhiều phần từ khác nhau trên website.
Vô tình chúng ta chặn luôn cả việc người dùng trải nghiệm trên website --> Điểm trừ tuyệt đối
Điểm thiệt hại còn hơn cả những việc nội dung bị copy.
Thật vậy, tôi chọn cách sử dụng win-win như sau :
## Đoạn code javaScript tự dán

- Tự dán cho dân DEV và người chuyên nghiệp
- Ngay cả các bạn mới biết dán code cũng có thể sử dụng

{% codeblock auto add link lang:javascript https://detusama.com Nguồn: Đệ Tứ Sama %}
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

## Hướng dẫn chèn code tự động dán link bài viết gốc