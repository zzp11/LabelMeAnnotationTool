
<!--#include virtual="..." --> 包含文件，虚拟路径
<!--#include ="..." -->

$('#myCanvas_bg_div').attr("onmousedown","javascript:StartDrawEvent(event);return false;"); 改变属性

$('#draw_canvas_div').unbind(); 解除绑定

$('#draw_canvas_div').mousedown({obj: this},function(e) {
      return DrawCanvasMouseDown(e.originalEvent);
    });     绑定事件