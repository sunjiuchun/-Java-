# StringBuilder

`StringBuilder`是一个可变对象，可以预分配缓冲区，
新增字符时，不会创建新的临时对象

	var sb = new StringBuilder(1024);
	sb.append("Mr ");
	  .append("Bob");
	  .append("!");
	  .insert(0, "Hello, ");
	System.out.pruintln(sb.toString());

`StringBuilder`源码中，定义的`append()`方法会返回
`this`，因此可以不断调用自身的其他方法


课后作业

	static String buildInsertSql(String table, String[] fields) {
        StringBuilder sb = new StringBuilder();
		
		sb.append("INSERT INTO "+table+" ("+fields[0]+", "
		+fields[1]+", "+fields[2]+")"+" VALUES (?, ?, ?)");

        return "";
    }