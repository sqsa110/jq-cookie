# jq-cookie
===
#操作说明<br> 
//设置cookie aa值为bb<br> 
  $.cookieOper('aa','bb');<br> 
//设置cookie bb值为cc  dd值为ee  ff值为gg<br> 
  $.cookieOper({bb:'cc',dd:'ee',ff:'gg'});<br> 
//设置cookie gg值为bb 时长1天<br> 
  $.cookieOper('gg','bb',1);<br> 
//设置xx值为cc yy值为ee zz值为gg 时长1天<br> 
  $.cookieOper({xx:'cc',yy:'ee',zz:'gg'},1);<br> 
//读取cookie aa和bb的值<br> 
  console.log($.cookieOper(['aa','bb']));<br> 
//读取cookie zz的值  <br> 
  console.log($.cookieOper('zz'));<br> 
//删除cookie bb和dd的值  <br> 
  $.cookieOper(['bb','dd'],true);<br> 
//删除cookie aa的值<br> 
  $.cookieOper('aa',true);<br> 
