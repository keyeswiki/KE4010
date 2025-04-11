# Arduino

## 1. Arduino简介  

Arduino是一种用于电子原型构建的开源平台，结合了硬件（Arduino开发板）和软件（Arduino IDE）。它广泛用于教育、创客运动和建筑原型，因其易用性和灵活性受到许多开发者和爱好者的喜爱。通过Arduino，用户可以轻松控制各种传感器和执行器，实现有趣的互动项目。  

Arduino的主要特点包括：  
- **开源性**：Arduino硬件和软件都是开源的，允许用户自由修改和分享。  
- **丰富的库**：提供大量的库和示例，帮助用户简化复杂任务。  
- **易于上手**：用户友好的编程环境，支持C/C++编程语言，适合初学者和经验丰富的开发者使用。  
- **跨平台**：Arduino IDE可以在多种操作系统上运行，包括Windows、macOS和Linux。  

## 2. 连接图  

![](media/868ccbea7a88e2c791e3e288264deca6.png)  

## 3. 测试代码  

```cpp  
int buzzPin = 3; // 定义数字口3  

void setup() {  
    pinMode(buzzPin, OUTPUT); // 将buzzPin设置为输出  
}  

void loop() {  
    digitalWrite(buzzPin, HIGH); // 有源蜂鸣器响起  
    delay(2000); // 延迟2S  
    digitalWrite(buzzPin, LOW); // 有源蜂鸣器关闭  
    delay(2000); // 延迟2S  
}  
```  

## 4. 测试结果  

有源蜂鸣器只需要高电平电压即可启动。在烧录好代码并连接好线后，上电后，有源蜂鸣器响起2秒，之后静音2秒，循环交替。




