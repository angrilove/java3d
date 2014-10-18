
import java.applet.Applet;
import java.awt.*;
import java.awt.event.*;

import com.sun.j3d.utils.applet.MainFrame;
import com.sun.j3d.utils.geometry.ColorCube;
import com.sun.j3d.utils.universe.*;
import javax.media.j3d.*;

public class HelloJava extends Applet {

	public HelloJava() {
		setLayout(new BorderLayout());
		Canvas3D c3d = new Canvas3D(null);
		add("Center", c3d);
		BranchGroup scene = createSceneGraph();
		scene.compile();
		SimpleUniverse su = new SimpleUniverse(c3d);
		su.getViewingPlatform().setNominalViewingTransform();
		su.addBranchGrop(scene);
	}

	public BranchGroup createSceneGraph() {
		BranchGroup root = new BranchGroup();
		root.addChild(new ColorCube(0.4));
		return root;
	}

	public static void main(String[] args) {
		Frame frame = new MainFrame(new HelloJava(), 256, 256);
	}
}
