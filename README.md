# EDSY with guardian engineering

This is how I think the guardian overhaul should be done, to make the grind of unlocking them worth while, improving base stats of some and adding engineering to them.

So this is a fork of the EDSY calculator, with numbers adjusted for guardian modules. Link to modified edsy: https://superartyk.github.io/EDSY_guardianEngineering/

Also at the same time adding the long-desired module reinforcement engineering. (Which makes me realise that hull tanking is not that bad, and honestly feel like *intentionally* nerfed.)

Because the game progression is currently this:

* Beginning of the game -- ship module progression with credits. Fun and straightforward
* Early mid-game -- player is done with module progression, finds out about guardian modules; (most) better than normal, player grinds them out. Mostly straightforward
* Mid-game to end of the game -- player find out about engineers that fine-tune modules to make them better compared to crude guardian hybrids. Mostly straightforward and easy to use (except materials, but a price to pay for performance

Add that's it. After mid-game there is no use for the hybrid guardian modules, hundreds of hours and a cool module ideas are lost. 

And some modules, like hull and module reinforcement or weapons offer little to no improvement to the standard module at the excessively large power draw--what's the point even?

And weapons unlocks aren't straightforward, nowhere does the game tell you that they are AX-specific, only outside resorces.

So, after playing with numbers and EDSY code, I propose:

* Early mid-game -- buff the base statistics of guardian hull and module reinforcements. 

* Late-game to end-game -- guardian hybrid module engineering (FSD and shield booster remain the same). Only after getting triple elite, unlocking at least 1 weapon and 1 hybrid module, and getting level 5 with: __Ram Tah, Zacariah Nemo, Tod McQuinn, Hera Tani, and The Dweller__. 
    * Guardian engineering to use guardian materials 
    * Guardian weapons, powerplant, and distributor all have normal engineering blueprints and experimentals (pre-engineered weapons cannot get experimentals)
    * "Heavy duty"-like blueprint on guardian hull and module reinforcements add additional power draw

* Add section in advanced maintenance menu to choose weapon ammo type. Label the current guardian weapon damage split (50/50 on human and AX) as "Anti-Xeno ammunition", and add the "Human ammunition" with 100% human damage
    * Human ammunition on Gauss and Shards to have 50% thermal (current) and 50% kinetic.
    * Human ammunition on Plasma to have 50% absolute (current), 25% thermal and 25% kinetic
    * Make the normal station restock and ship ammo synthesis for guardian weapons to replenish the last selected ammo type

* With changes to ammo, make the ship only apply limit of 4 to guardian weaponry only if Anti Xeno damage is selected (to align with other anti xeno weapons) 

And it makes sense, and gives logical end to the progression, tying up the previous time spent grinding out the guardian modules and using the player's knowledge.

It makes sense that hybrid modules would be better than stock, theoretically, since guardians are a highly intelligent race and their technology vastly outperforms our own.

And from the balance perspective, that fine-tuned human modules to outperform the crude hacks with guardian technolgy makes sense too.

And the pinnacle of the technology, fine tuning the vastly-superior guardian modules to prove much better than human ones, at cost of more grinding for materials and unlocks. 

It feels more rewarding, and less like a complete waste of time. And in the end guardian modules aren't always better, they eat more power, produce more heat, and weapons use more distributor. 

Which requires the knowledge of the equpment of the pilot, which works at this stage of the game.



# So. List of changes and my proposal to fix guardians and engineering:

### I have not added proper material requirements for blueprints yet!

* Guardian Hull and Module Reinforcements are now 1.5x the human counterpart (instead of 1.25x) to feel more rewarding for the grind and energy requirement.
    
	* 1.35x they start to seem not as much underwhelming (engineering with that is a bit meh), 1.4x they look somewhat okay, 1.45x seem attractive, 1.5x is perfect (while the raw stats like Integrity seem to be high, the lack of Resistances makes up for that)
    
		* Additionally the 1.5x helps to use it to allow hull-tanking to be closer to shield-tanking
		
    * This also brings them to the trend of guardian modules being grade 3 engineering of human ones

* Guardian modules have engineering working for them
    * Guardian Hull Reinforcement gets 40% more power draw on Heavy Duty blueprint, 15% on resistance blueprints, and -24% on light-weight

* Added module reinforcement engineering (pls suggest better names):
    * "Fortified Lattice": 250% increase in integrity at 100% more mass and -40% protection percentage
        * 60% on D-rated turns into 39% (3x of those turn to 77% instead of 94% protection)
        * 5D MRP has 350 integrity, with this modification: 1225
            
			* While this integrity might seem excessive, this is a counterpart to shield tanking and engineering (which counteract the hulltank by module sniping), where shield boosters get **ADDITIVE** increase in reinforcement for heavy duty, achieving over **3X** the improvement with grade 5 Heavy Duty.
        
		* Guardian MRP's have additional 100% power draw
            * Guardian 5D MRP turns 525 integrity into 1837.5

    * "Ablative Sheathing": 30% increase in protection% at the cost of 30% more mass and -20% integrity
        * 60% on D-rated, turns into 78%, 3x of those turn to 99%
        * Guardian MRP's have additional 40% power draw

* EDSY-specific change: Removed "illegal" blueprints from guardian weapons, to not allow to engineer for them
    
	* This somewhat breaks the EDSY blueprints names showing on guardian pre-engineered modules, now showing a different blueprint. This is just a visual change, stats stay the same.
  

