**FileInputStream**

```
package io;

import java.io.FileInputStream;
import java.io.FileNotFoundException;
import java.io.IOException;

public class IoDemo1 {
    public static void main(String []args) {
        FileInputStream fis=null;
        try {
            fis=new FileInputStream("C:/Users/xj/Desktop/demo.txt");
            byte[]bytes=new byte[4];
            while(true){
                int readCount=fis.read(bytes);
                if(readCount==-1){
                    break;
                }
                System.out.print(new String(bytes,0,readCount));
            }
        } catch (FileNotFoundException e) {
            e.printStackTrace();
        } catch (IOException e) {
            e.printStackTrace();
        } finally {
            if(fis!=null){
                try {
                    fis.close();
                } catch (IOException e) {
                    e.printStackTrace();
                }
            }
        }
    }


}

```

