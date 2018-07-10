# Orb-Run

## Scripts:
*	CameraPositioner
*	Collectible
*	CollectibleCreator
*	Collectibles
*	ExplosionSimulator
*	GameController
*	Repository
*	SelfRotator
*	SoundController
*	TrailSystem
*	TriggerEnterNotifier
*	TriggerExitNotifier
*	UIManager

## Key script behavior:
### GameController
*	The only controller script with update loop in the ‘OrbRun’ scene.
*	Master controller of the following entities: 
*	camera, sound controller, UI Manager, trail system, explosion simulator, collectibles
*	Responsible for processing user inputs.
*	Controls all the main events taking place in the game.
*	Controls the projectile gun.

### CollectibleCreator
*	Creates collectibles and places them on the slider based on the simulated orb movement.
*	It also stores references to the ‘Collectible’ script instances at the time of creation into instance of another script ‘Collectibles’. This saves the time to get the references during gameplay.

### Repository
*	Single static class that keeps track of information like reference to GameController, constants and user’s score information.
*	Avoids complex ‘public reference’ wiring between scripts. Especially during collision events.

## Future improvements:
*	Improve the UI screens, add clickable buttons and add more functionality.
*	Effects (like explosion) and camera angles could be enhanced.
*	Definitely replace the first slider (corresponding to the first portal). Because of the bumps in the slider it could lead to erratic behavior.
*	Review the topology of 3D objects and their collision meshes.
*	Add more comments to the code.
*	Refactor the code.

## External assets used:
*	Low poly globe.
*	Slider – 3D models.
*	Cannon – 3D model.
*	The island terrain.
*	Sound effects.
*	Text-mesh pro for UI textfields.
*	Textures.


