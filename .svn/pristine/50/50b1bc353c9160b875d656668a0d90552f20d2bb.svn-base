/*
 * To change this template, choose Tools | Templates
 * and open the template in the editor.
 */
package com.thando.assignment;

import com.thando.Assignment.conf.AppConfig;
import com.thando.Assignment.services.MainInterface;
import java.util.ArrayList;
import java.util.Arrays;
import java.util.List;
import org.springframework.context.ApplicationContext;
import org.springframework.context.annotation.AnnotationConfigApplicationContext;
import org.testng.Assert;
import static org.testng.Assert.*;
import org.testng.annotations.AfterClass;
import org.testng.annotations.AfterMethod;
import org.testng.annotations.BeforeClass;
import org.testng.annotations.BeforeMethod;
import org.testng.annotations.Test;

/**
 *
 * @author 210119578
 */
public class ArrayTest {
    private static MainInterface callinObj;
      private static ApplicationContext ctx;
    
    public ArrayTest() {
    }
    
     @Test
    public void TestArrayEquality() {
         
         List data =callinObj.getArray();
         
        List<String> names =new ArrayList<String>(Arrays.asList("thando","210119578"));
        
         
         Assert.assertEquals(data,names, "these arrays are not the same");
     }

    @BeforeClass
    public static void setUpClass() throws Exception {
        
         ctx = new AnnotationConfigApplicationContext(AppConfig.class);
        callinObj = (MainInterface)ctx.getBean("arrays");
    }

    @AfterClass
    public static void tearDownClass() throws Exception {
    }

    @BeforeMethod
    public void setUpMethod() throws Exception {
    }

    @AfterMethod
    public void tearDownMethod() throws Exception {
    }
}
