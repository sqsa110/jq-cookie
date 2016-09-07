# jq-cookie \n
操作说明  \n
//设置cookie aa值为bb
  $.cookieOper('aa','bb');
//设置cookie bb值为cc  dd值为ee  ff值为gg
  $.cookieOper({bb:'cc',dd:'ee',ff:'gg'});
//设置cookie gg值为bb 时长1天
  $.cookieOper('gg','bb',1);
//设置xx值为cc yy值为ee zz值为gg 时长1天
  $.cookieOper({xx:'cc',yy:'ee',zz:'gg'},1);
//读取cookie aa和bb的值
  console.log($.cookieOper(['aa','bb']));
//读取cookie zz的值  
  console.log($.cookieOper('zz'));
//删除cookie bb和dd的值  
  $.cookieOper(['bb','dd'],true);
//删除cookie aa的值
  $.cookieOper('aa',true);
