
### 包含脚本文件，虚拟路径
    <!--#include virtual="..." -->
    <!--#include ="..." -->

### 改变属性
    $('#myCanvas_bg_div').attr("onmousedown","javascript:StartDrawEvent(event);return false;"); 

### 解除绑定
    $('#draw_canvas_div').unbind(); 

### 绑定事件
    $('#draw_canvas_div').mousedown({obj: this},function(e) {
      return DrawCanvasMouseDown(e.originalEvent);
    }); 

### 通过插入元素来画线
    $('#'+element_id).append('<a xmlns="http://www.w3.org/2000/svg"> <polyline xmlns="http://www.w3.org/2000/svg" id="' + dom_id + '" points="' + poly_points + '" ' + attr + ' /></a>');
