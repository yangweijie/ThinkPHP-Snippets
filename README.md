ThinkPHP-Snippets
=================

Code snippets for developing with ThinkPHP framework

The plugin give you 3 places to generate code(template eg: *.html ,action & model eg: *.php.) 

Here are all the snippets stand for:
 str,tab -> [source code]
	*.html:
		:,tab ->{:fun()}
		layout,tab -><include file="Public:header"/>
{__CONTENT__}
<include file="Public:footer"/>
		php,tab -> <php>echo 'Hello,world!';</php>
		|fun,tab -> {$name|fun=arg1,###}
		|def,tab -> {$name|default="***"}
		$.tab -> {$name}
		emp,tab -> <empty name="name">name为空<else /> name不为空</empty>
		eq,tab -> <eq name="name" value="value">value</eq>
		inc,tab -> <include file="Public:header" />
		nolayout,tab -> {__NOLAYOUT__}
		pre,tab -> <present name="name">name已经赋值<else />name还没有赋值</present>
		switch,tab -> <switch name="User.level">
	<case value="1">value1</case>
	<case value="2">value2</case>
	<default />default
</switch>
		vo,tab -> <volist name="list" id="vo">
	{$key}.{$vo.name}
</volist>
	*.php:
		Action,tab -> Class IndexAction extends Action{
							public function index}(){
								
							}
					     }
		auto,tab -> protected $_auto = array ( 
	array('status','1'),  // 新增的时候把status字段设置为1
	array('password','md5',1,'function') , // 对password字段在新增的时候使md5函数处理
	array('name','getName',1,'callback'), // 对name字段在新增的时候回调getName方法
	array('create_time','time',2,'function'), // 对create_time字段在更新的时候写入当前时间戳
);
		Model,tab -> Class $NewModel extends Model{
	
}
		table,tab -> protected $tablePrefix
		true,tab -> protected $trueTableName
		val,tab -> protected $_validate = array(
	array('verify','require','验证码必须！'), //默认情况下用正则进行验证
	array('name','','帐号名称已经存在！',0,'unique',1), // 在新增的时候验证name字段是否唯一
	array('value',array(1,2,3),'值的范围不正确！',2,'in'), // 当值不为空的时候判断是否在一个范围内
	array('repassword','password','确认密码不正确',0,'confirm'), // 验证确认密码是否和密码一致
	array('password','checkPwd','密码格式不正确',0,'function'), // 自定义函数验证密码格式
);
		_a,tab ->protected function _after_delete($data,$options) {
					
				   }
		_a,tab -> protected function _after_find(&$result,$options) {
						
				   }
	   	_a,tab -> protected function _after_insert($data,$options) {
					
				    }
	    	_a,tab -> protected function _after_update($data,$options) {
						
				    }
	    	_b,tab -> protected function _before_insert(&$data,$options) {
			 
				    }

		_b,tab -> protected function _before_update(&$data,$options) {
				 
				    }
	    	$this-> -> $this->ajaxReturn($data,$info,$status,$type);
	    	$this-> ->$this->assign('name',$name);
	    	$this-> -> $this->display();
	    	$this-> -> $this->error();
	    	$this-> -> $this->fetch();
	    	$this-> -> $this->getActionName();
	    	$this-> -> $this->isAjax();
	    	$this-> -> $this->isDelete();
	    	$this-> -> $this->isGet();
	    	$this-> -> $this->isHead();
	    	$this-> -> $this->isPost();
	    	$this-> -> $this->isPut();
	    	$this-> -> $this->redirect($url,$params,$delay,$msg);
	    	$this-> -> $this->success();
	    	$this-> -> $this->_empty();
	    	this-> -> $this->_post();
	    	$this-> -> $this->_get($name);
		->,tab -> ->_sql();
		->,tab -> ->addAll($dataList,$options,$replace);
		->,tab -> ->alias();
		->,tab -> ->avg();
		->,tab -> ->buildSql();
		->,tab -> ->commit();
		->,tab -> ->count();
		->,tab -> ->create();
		->,tab -> ->delete();
		->,tab -> ->distinct();
		->,tab -> ->execute();
		->,tab -> ->field();
		->,tab -> ->find();
		->,tab -> ->getDbError();
		->,tab -> ->getError();
		->,tab -> ->getField($field,$value);
		->,tab -> ->getModelName();
		->,tab -> ->group();
		->,tab -> ->having();
		->,tab -> ->limit();
		->,tab -> ->lock();
		->,tab -> ->max();
		->,tab -> ->min();
		->,tab -> ->order();
		->,tab -> ->page();
		->,tab -> ->query();
		->,tab -> ->rollback();
		->,tab -> ->selectAdd();
		->,tab -> ->setField();
		->,tab -> ->setInc();
		->,tab -> ->setProperty();
		->,tab -> ->startTrans();
		->,tab -> ->sum();
		->,tab -> ->switchModel();
		->,tab -> ->where();
		->,tab -> ->table();





