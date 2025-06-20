## 🔍 Overview
The life cycle of an applet is managed by the **browser** or **applet viewer**. It consists of a series of method calls that define the different stages of an applet's life.

## 🧬 Life Cycle Stages

### 1. `init()`
- Called **once** when the applet is first loaded.
- Used for **initialization**, like setting up UI components or loading resources.

### 2. `start()`
- Called **each time** the applet becomes visible/active (e.g., when the user returns to the page).
- Start or **resume** ongoing tasks such as animations or threads.

### 3. `paint(Graphics g)`
- Called when the applet needs to **redraw** its content.
- Used for displaying UI elements, drawing shapes, strings, etc.

### 4. `stop()`
- Called when the applet is **no longer active** (e.g., user navigates away).
- Pause any ongoing actions like music, animation, threads.

### 5. `destroy()`
- Called when the applet is being **unloaded** from memory.
- Used to **release resources** (e.g., close files, threads, network connections).

---
## 🔄 Life Cycle Flow
![[Pasted image 20250619211608.png]]


**Expample:**
``` java
import java.applet.Applet;
import java.awt.Graphics;

public class MyApplet extends Applet {
  public void init() {
    System.out.println("Applet initialized");
  }

  public void start() {
    System.out.println("Applet started");
  }

  public void paint(Graphics g) {
    g.drawString("Hello Applet!", 50, 50);
  }

  public void stop() {
    System.out.println("Applet stopped");
  }

  public void destroy() {
    System.out.println("Applet destroyed");
  }
}
```
