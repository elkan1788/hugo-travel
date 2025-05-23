---
date: '2025-05-23T18:50:07+08:00'
draft: false
tags:
- wihte
title: 'Code Block'
---

Anim eiusmod irure incididunt sint cupidatat. Incididunt irure irure irure nisi ipsum do ut quis fugiat consectetur proident cupidatat incididunt cillum. Dolore voluptate occaecat qui mollit laborum ullamco et. Ipsum laboris officia anim laboris culpa eiusmod ex magna ex cupidatat anim ipsum aute. Mollit aliquip occaecat qui sunt velit ut cupidatat reprehenderit enim sunt laborum. Velit veniam in officia nulla adipisicing ut duis officia.

Use Hugo inside take style for code block display. :smile: :tada:

{{< highlight go "linenos=table,hl_lines=8 15-17,linenostart=199" >}}

func GetTitleFunc(style string) func(s string) string {
  switch strings.ToLower(style) {
  case "go":
    return strings.Title
  case "chicago":
    return transform.NewTitleConverter(transform.ChicagoStyle)
  default:
    return transform.NewTitleConverter(transform.APStyle)
  }
}

{{< / highlight >}}

markdown code block style：

```java
import javax.swing.JFrame;  //Importing class JFrame
import javax.swing.JLabel;  //Importing class JLabel
public class HelloWorld {
  public static void main(String[] args) {
    JFrame frame = new JFrame();           //Creating frame
    frame.setTitle("Hi!");                 //Setting title frame
    frame.add(new JLabel("Hello, world!"));//Adding text to frame
    frame.pack();                          //Setting size to smallest
    frame.setLocationRelativeTo(null);     //Centering frame
    frame.setVisible(true);                //Showing frame
  }
}
```