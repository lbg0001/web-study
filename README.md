# web-study
my first repository on GitHub
class Student
	{
		//定义成员属性
		public $name=NULL;
		public $Student_id=NULL;
		public $age=NULL;
		//定义成员方法
		public function introduce()
		{
			//echo '我是'.'{$this->name}';
			echo "我是{$this->name}";
		}
		
	}
  
  //实例化
  header('content-type:text/html;charset=utf-8');
	require './student.class.php';
	$student1= new Student();
	var_dump($student1);
	echo '<br />';
	$student1->name="小明";
	$student1->Student_id="20180001";
	$student1->age=18;
	echo '<br />';
	var_dump($student1);
	$student1->introduce();
