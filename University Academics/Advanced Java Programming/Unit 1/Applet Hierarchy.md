#### AWT based Applet Hierarchy
``` 
java.lang.Object
   └── java.awt.Component
         └── java.awt.Container
               └── java.awt.Panel
                     └── java.applet.Applet

```


1. **Object:** Root of all Java Classes.
2. **Component:** An abstract class for all AWT UI elements like Button, textfield.
3. **Container:** A component that can contain other components like panes, frames.
4. **Panel:** A generic container, used to group components.
5. **[[Applet]]:** The main class for creating applets using AWT. It provides the base structure for [[Applet life cycle]] methods.