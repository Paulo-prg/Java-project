# Java-project
import java.applet.AudioClip;
import java.awt.HeadlessException;
import java.net.URL;
import javax.swing.JButton;
import javax.swing.JFrame;
import static javax.swing.JFrame.EXIT_ON_CLOSE;

/**
 *
 * @author paulf
 */
public class JavaApplication9 extends JFrame {

 JButton tocar;

       

    public JavaApplication9(){
    
        tocar = new JButton("Voz de teste");
        
                setDefaultCloseOperation(EXIT_ON_CLOSE);
                setSize(200,200);
                setLocationRelativeTo(null);
                setVisible(true);
                
                add(tocar);
                tocar.addActionListener(new ActionListener){
        public void actionPerformed(Actionevent e){
                play(Silvio);
            
        }
    };
                
} 
                
            
        }
    
    public void play(String nomeDoAudio) {
             URL url = getClass().class.getResource(nomeDoAudio+".wav");
            AudioClip audio = applet.newAudioClip(url);
            audio.play();
    }

    private static void main(String[]args){
        
new TocarSom();
        
        }

    private static class applet {

        private static AudioClip newAudioClip(URL url) {
            throw new UnsupportedOperationException("Not supported yet."); // Generated from nbfs://nbhost/SystemFileSystem/Templates/Classes/Code/GeneratedMethodBody
        }

        public applet() {
        }
    }
