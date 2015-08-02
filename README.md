# Gmail.
package com.gmail.test;

import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.firefox.FirefoxDriver;
import org.openqa.selenium.support.ui.ExpectedCondition;
import org.openqa.selenium.support.ui.ExpectedConditions;
import org.testng.annotations.Test;

public class GmailLogin {
	 
//driver.ger("http//google.com");
	
  @Test
  public GmailLogin() {
	  WebDriver driver = new FirefoxDriver();
	  driver.get("http://google.com");
	  driver.findElement(By.id("gb_70")).click();
	  driver.findElement(By.name("Email")).sendKeys("drp2925");
	  driver.findElement(By.id("next")).click();
	  until(ExpectedConditions.presenceOfElementLocated(By.name("Passwd")));
	  driver.findElement(By.id("Passwd")).sendKeys("Jalaram23");
	 // driver.findElement(By.xpath("form/div[2]/div/div[2]/div/div/input[2]")).sendKeys("bittu292518");
	  //driver.findElement(By.id("signIn")).click();	
  }

private void until(ExpectedCondition<WebElement> presenceOfElementLocated) {
	// TODO Auto-generated method stub
	
}
}
