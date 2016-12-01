# EEG_T-Stress

##WHO:
- Aniela Hoitink; Fashion and Textile Designer 
- Esmee Lim; Concept Designer 
- Inês Palma de Lima e Cruz; Technology Expert 
- Irene Gielen; Communications Expert 
- Martin Walchshofer; Developer 

##WHY
The modern open office was designed for team building and camaraderie but is mostly distinguished by its high noise levels, lack of privacy and surfeit of both digital and human distractions. And indeed, several decades of research have confirmed that open-plan offices are generally associated with greater employee stress, poorer co-worker relations and reduced satisfaction with the physical environment. But there are some ways to combat those detrimental effects and still be productive. Frequently alternating between helping colleagues and doing one’s own job imposes a heavy cognitive load, as the help givers are forced to repeatedly reacquaint themselves with the details of their own task. Stress in the workplace leads to high staff turnover, loss of productivity and high absenteeism.
 The T-Stress signals when employees are stressed. Their managers then know that actions are required to manage the team stress levels.

##WHAT
The T-Stress is a piece of clothing that is easy to wear for office employees. It signals when someone’s stress level is high by measuring the person’s EEG and translating it into the clothing color.

![image 1](https://github.com/HackTheBrain/EEG_T-Stress/blob/master/images/Schermafbeelding%202016-12-01%20om%205.22.15%20p.m..png)
##Figuur 1 Sewing action

##WHAT WE EXPECTED TO HAPPEN
For the T-Stress to work, certain properties in the EEG that correlate to stress must be found.
According to literature, some stress correlates have been found in the beta and alpha frequency bands on central and frontal sites. Furthermore if we look through the emotional aspect, stress can be translated into an unpleasant and high arousal feeling which has also been linked to frontal alpha and other frequency changes in frontal/central sites.
To test out theory, we executed a simples stress test by submerging the subject’s hand into ice water for a little under a minute after a baseline was established and recorded. We analyzed data in the frequency spectrum, averaging the data across 2 second epochs.
For this we choose a g.Nautilus - g.tec's wireless EEG system with 16 dry electrodes due to its good signal quality and easiness to put on-and-off. 

*Figuur 2 stress test*

Although we expected to see some changes between the two conditions (see below figure), that didn’t happen immediately and more careful EEG exploration would have to be done. 

*Figuur 3 Power spectrum averaged across 2 second windows for baseline condition (top) and stress condition (bottom)*

##WORKING PROTOTYPE
Our final prototype provides a link between the person’s direct EEG signals and the LED colors. 
Over the weekend we tested several approaches on how to connect g.Nautilus with arduino:
g.Nautilus  BCI2000  UDP  Any programming language that supports UDP sockets (Matlab, C#, Python, Java,… and many more)  Any other device (Arduino, other BCI etc.)
g.Nautilus  OpenVibe  UDP  Any programming language that supports UDP sockets (Matlab, C#, Python, Java,… and many more)  Any other device (Arduino, other BCI etc.)
g.Nautilus  g.tec GDS API available for C/C++ , C# (requires an windows server)  Any other device (Arduino, other BCI etc.)
g.Nautilus  Matlab / g.tec Highspeed Online Processing Library  Any other device (Arduino, other BCI etc.)

The LEDs are positioned so that they are clearly visible on the back of someone in an office chair. 
Figuur 4 LED's

##SOURCES:
Brennan A, Chugh JS, Kline T. Traditional versus open office design: A longitudinal field study. Environment and behavior. 2002 2002;34:279–99. 
Oommen, V, Knowles, M, & Zhao, I. Should health service managers embrace open plan work environments? A review. Asia Pacific Journal of Health Management. 2008, 3(2), pp. 37-43.


