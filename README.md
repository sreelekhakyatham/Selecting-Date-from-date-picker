//# Selecting-Date-from-date-picker

package Webdriver;

import org.openqa.selenium.By;
import org.openqa.selenium.Keys;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.chrome.ChromeDriver;

public class Selecting_Date_From_DatePicker 
{

	public static void main(String[] args) throws Exception 
	{
		WebDriver driver=new ChromeDriver();
		driver.get("https://jqueryui.com/resources/demos/datepicker/dropdown-month-year.html");
		driver.manage().window().maximize();
		
		driver.findElement(By.id("datepicker"));
		Thread.sleep(1000);
		
		driver.findElement(By.id("datepicker")).clear();
		driver.findElement(By.id("datepicker")).sendKeys("10/05/2024"+Keys.ESCAPE);
		

	}

}
