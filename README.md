# in-class-activities
## Devlogs
### W1
The camera won't follow the cat anymore
https://zukangz.itch.io/1

### W2
1.Because they are fractional numbers.
2.Because _bounce is whole number without floats
3.It didn't have a ;

### W3
Part1
1.Parameters(input): current friendship level+if your character knows the character’s secret;We need these two pieces of information to decide what line the character should say. Without them, the game cannot pick the right dialogue.
  return type(output):a line of text;The whole purpose of this method is to return the character’s spoken reply.
2.Parameters(input):sanity level;The brightness of the room’s light changes based on the player’s sanity value. The method needs this number to know how dim or bright to set the lights.
  return type(output):void;This method directly modifies the light in the game. It does not need to send any data back to other code after finishing its work.
3.Parameters(input):the time you press the key;The game must compare this exact press time against the target beat time to check for a hit.
  return type(output):true or false;We only need a simple yes‑or‑no answer to tell if the player hit the beat correctly.

Part2
My metaphor for classes and components is a cookie cutter. The class is the cookie cutter template, and components are the individual cookies stamped out from it. Member variables are the cookie’s traits like size and number of chocolate chips. Methods are actions the cookie can perform, such as baking or adding sprinkles. One template (class) can create many unique cookies (components).

Part3
Because each bounce overwrite the RGB repeatedly.

### W4
Table 9
I add colliders to cat and soccer ball.The soccer ball is trigger on the goal.
My game runs well

### W5
1.A variable to store the position of the target GameObject the deer will walk towards. It needs to be a Transform and must have the [SerializeField] attribute so it can be tuned in the Inspector.
2.Start() 
  Update()
3.Start(): It should use GetComponent<NavMeshAgent>() to find the NavMeshAgent component attached to the Deer and assign it to the agent variable.
Update(): It should use the agent variable to continuously tell the deer where to walk by calling agent.SetDestination. This ensures the deer keeps walking towards the target as long as the game is running.


### MG3
int:0 float:0.0f bool:false string:null 
Update()is a Unity built-in message function.Unity automatically calls Update() once every frame.Should not be manually called Update() in the code. The Unity engine invokes it automatically.
The Timer class handles counting down time.
1. We call BeginTimer() to start the timer and set its total duration.
2. Inside the Update() method of KickWeapon / GameManager, we check the timer every frame with IsFinished().
3. If IsFinished() returns true, we run our logic: disable the kick weapon object or trigger GameOver.
4. The Update() method runs every frame, so we can continuously check the timer state.
## Open-Source Assets
### W1
- Animals: https://assetstore.unity.com/packages/3d/characters/animals/animals-free-animated-low-poly-3d-models-260727 
- Low-poly environment: https://assetstore.unity.com/packages/3d/environments/landscapes/low-poly-simple-nature-pack-162153 
