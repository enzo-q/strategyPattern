# strategyPattern
<h3>Software Engineering 2 | Lab Assignment 1</h3>
<h3>Problem Scenario:</h3>

Suppose we have three types of characters in a GameApp:

1. Knight: Attacks with a sword; uses 3 strategies to defend (shield, dodge, magic barrier)
2. Wizard: Casts spells; uses magic barrier to defend
3. Archer: Shoots arrows; uses dodge to to defend

Implement two types of Strategy:

A.  DefenseStrategy
<ul>
<li>Shield</li>
<li>Dodge</li>
<li>CreateMagic</li>
</ul>

B.  AttackStrategy
<ul>
<li>CastSpell</li>
<li>ShootArrow</li>
<li>SwingSword</li>  
</ul>

Refactor the existing codes and provide the UML Diagram:

public class Character {
    private String type;
    
    public Character(String type) {
        this.type = type;
    }

    public void attack() {
        if (type.equals("Knight")) {
            System.out.println("Knight attacks with a sword!");
        } else if (type.equals("Wizard")) {
            System.out.println("Wizard casts a spell!");
        } else if (type.equals("Archer")) {
            System.out.println("Archer shoots an arrow!");
        }
    }

    public void defend() {
        if (type.equals("Knight")) {
            System.out.println("Using a shield to defend!");
	          System.out.println("Dodgin to avoid attack!");
            System.out.println("Creating a magic barrier for defense!"");		
        } else if (type.equals("Wizard")) {
            System.out.println("Creating a magic barrier for defense!"");
        } else if (type.equals("Archer")) {
            System.out.println("Using a shield to defend!"");
        }
    }
}

<h3>UML Class Diagram:</h3>
<img width="3647" height="1997" alt="GA_UML" src="https://github.com/user-attachments/assets/1c791604-a7af-4738-a23a-75c62bf0b59c" />
