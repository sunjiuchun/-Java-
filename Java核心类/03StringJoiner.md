# StringJoiner

StringJoiner

利用分隔符拼接数组

	String[] names = {"Bob", "Alice", "Grace"};
	var sj = new StringJoiner(", "，"Hello ","! ");//var定义一个变量
	for(String name : names){
		sj.add(name);
	}
	System.out.println(sj.toString());

String.join()

在不需要"开头/结尾"的时候，用String.join()更方便

	String[] names = {"Bob", "Alice", "Grace"};
	var s = String.join(", ", names);
