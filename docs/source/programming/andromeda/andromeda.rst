AndromedaLib
============

What is AndromedaLib?
---------------------

**Cheatsheet**

https://sphinx-tutorial.readthedocs.io/cheatsheet/

AndromedaLib is a library designed for making FRC programming far easier than before. Why? Because it includes many wrappers around many of WPILIB's classes to manage hardware.

For example, lets revisit how a CANSparkMax object is created using WPILIB's standard library: 

.. code-block:: java

    public class Robot extends TimedRobot {
        CANSparkMax spark1 = new CANSparkMax(2, MotorType.kBrushless);

        @Override
        public void robotInit(){
            spark1.setInverted(true);
            spark1.setSmartCurrentLimit(40);
            spark1.burnFlash();                
        }
    }

As you can see, there are several steps involved in creating and modifying how a specific motor works and interacts with the rest of the robot. Now, imagine having more than 10 motors being used, each would need to be defined and initialized in several lines, leading to bulky, unnecesary code. 

This is were AndromedaLib functions best. It includes many wrappers that allow multi-modifications via a single initalization in the following manner:

.. code-block:: java

    public class Robot extends TimedRobot {
        SuperSparkMax superSpark1 = new SuperSparkMax(3, GlobalIdleMode.Coast, true, 40);

        @Override
        public void robotInit(){
                
        }
    }

Therefore, we use instantiate a SuperSparkMax object with an id of 3, a coast idle mode, inverted, and with 40 amps of current limit. All of this through a single line.