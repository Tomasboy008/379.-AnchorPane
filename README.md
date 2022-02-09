# 379.-AnchorPane
Ancoragem de elementos a partir de referencias de Topo,Esq,Dir....
INICIO
__________________________
package layout;

import javafx.geometry.Pos;
import javafx.scene.layout.AnchorPane;
import javafx.scene.layout.HBox;

public class TesteAnchorPane extends AnchorPane{
	
	public TesteAnchorPane() {
	
		Quadrado q1 = new Quadrado();
		setTopAnchor(q1, 10.0);
		setLeftAnchor(q1, 10.0);
		
		Quadrado q2 = new Quadrado();
		setTopAnchor(q2, 10.0);
		setRightAnchor(q2, 10.0);
		
		Quadrado q3 = new Quadrado();
		setBottomAnchor(q3, 10.0);
		setLeftAnchor(q3, 10.0);
		
		Quadrado q4 = new Quadrado();
		setBottomAnchor(q4, 10.0);
		setRightAnchor(q4, 10.0);		

		HBox centro = new HBox();
		centro.setAlignment(Pos.CENTER);
		setTopAnchor(centro, 110.0);
		setBottomAnchor(centro, 110.0);
		setLeftAnchor(centro, 110.0);
		setRightAnchor(centro, 110.0);
		
		Quadrado q5 = new Quadrado();
		centro.getChildren().add(q5);
		
		getChildren().addAll(q1, q2, q3, q4, centro);
	}
}
![image](https://user-images.githubusercontent.com/95525963/153303015-4575f2f4-8ec8-4e87-95da-a57da412b74d.png)

Puxando as Bordas
_________________________

![image](https://user-images.githubusercontent.com/95525963/153303201-4317b263-719b-4220-9c93-23a8afcac79a.png)

