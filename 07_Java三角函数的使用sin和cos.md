# Java三角函数的使用`sin`和`cos`

- 使用`java.lang.Math`类来调用三角函数`sin`和`cos`

- 这些函数接受**参数的弧度值**，如果您有角度值，需要先将其转换为弧度`Math.toRadians()`

- 以下是如何在Java中调用这些函数的示例：

	```java
	import java.lang.Math;
	
	public class TrigonometryExample {
	    public static void main(String[] args) {
	        // 角度值
	        double degrees = 45.0;
	        
	        // 将角度转换为弧度
	        double radians = Math.toRadians(degrees);
	        
	        // 计算正弦值
	        double sinValue = Math.sin(radians);
	        
	        // 计算余弦值
	        double cosValue = Math.cos(radians);
	        
	        // 输出结果
	        System.out.println("The sine of " + degrees + " degrees is: " + sinValue);
	        System.out.println("The cosine of " + degrees + " degrees is: " + cosValue);
	    }
	}
	```

- 注意：在上述代码中，`Math.toRadians(degrees)`用于**将角度值转换为弧度**，因为`Math.sin`和`Math.cos`方法期望接收弧度作为参数