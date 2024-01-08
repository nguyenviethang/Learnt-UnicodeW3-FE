# học vè css
cấu trúc cú pháp:
selector {
    property1: value1;
    property2: value2;
}
lưu ý: 
- CSS có tính chất "Cascading", tức là các quy tắc có thể được ghi đè theo thứ tự ưu tiên.
- cách đặt tên id: class
    + tường minh
    + tiếng anh(đúng chính tả, dùng số ít và nhiều)
    + Viết thường, sử dụng gạch ngang, không nên dùng số
    + Nên bắt đầu bằng chữ cái
    + Cháp nhận: chữ cái thường, dấu gạch dưới, gạch ngang, số
    + Không được phép bắt đầu bằng số
    + Sử dụng danh từ 
    + id trong 1 thẻ chỉ có 1
    + class trong 1 thẻ html sẽ có nhiều (Mỗi class sẽ cách nhau bởi khoảng trắng)

Nguyên tắc với selector ~

- Cùng cấp
- Nằm trong 1 cha
- Không phân biệt thứ tự liền sau

## tìm hiểu cách sự dung selector phổ biến

 ### cách 1: id, class, element HTML,
    Selector của lớp (Class Selector): .class-name { }
    Selector của ID: #id-name { }
    Selector phần tử HTML: element { }
    Selector kết hợp: element.class { }, element#id { }, elementA elementB { }, v.v.


    vi du về selector ket hợp:
    /* Selector phần tử kết hợp với class */
    element.class-name { /* Áp dụng cho các phần tử có class "class-name" là con của phần tử element */
    /* CSS properties */
    }

    /* Selector phần tử kết hợp với ID */
    element#id-name { /* Áp dụng cho phần tử có ID là "id-name" là con của phần tử element */
        /* CSS properties */
    }



### cách 2: Selector con, người em, người anh:
    Chọn tất cả các phần tử: * { }
    Chọn tất cả các phần tử con của một phần tử: parent > child { }
    Chọn phần tử ngay kế tiếp: element + next-element { }
    Chọn phần tử cùng loại: element ~ sibling-element { }


ví dụ:

/* Lựa chọn tất cả các phần tử <a> là con của các phần tử <li> */
li > a {
    /* CSS properties */
}

/* Lựa chọn phần tử ngay kế tiếp sau phần tử <h2> */
h2 + p {
    /* CSS properties */
}

/* Lựa chọn tất cả các phần tử em (siblings) của phần tử */
h2 ~ p {
    /* CSS properties */
}

### cách 3: Selector thuộc tính: chọn các element html có attribute cụ thẻ
ví dụ :

/* Chọn tất cả các phần tử có thuộc tính "target" */
[target] {
    /* CSS properties */
}

/* Chọn các phần tử có thuộc tính "target" với giá trị "blank" */
[target="_blank"] {
    /* CSS properties */
}

### cách 4: Selector pseudo-class và pseudo-element: Chọn các trạng thái hoặc phần tử cụ thể:

ví dụ: 
/* Selector pseudo-class cho phần tử khi rê chuột qua */
a:hover {
    /* CSS properties */
}

/* Selector pseudo-element chọn phần tử đầu tiên trong một loại phần tử */
p:first-of-type {
    /* CSS properties */
}




