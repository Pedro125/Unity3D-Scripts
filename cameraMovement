using UnityEngine;
using System.Collections;

public class cameraMovement : MonoBehaviour
{
	//Variables
	public static string forward = "up";
	public static string right = "right";
	public static string down = "down";
	public static string left = "left";

	public static int movementSpeed = 5;

	public static int mapSize = 200;

	public static bool cameraMove

	void Start()
	{
		mapSize = mapSize / 2;
		//since the map will be centered at (0,0,0) , we need to divide the map size by two
	}

	void Update ()
	{

		if ((Input.GetButton(forward)) && canCameraMove(forward)) {
			transform.Translate (0, 0, movementSpeed * Time.deltaTime);
		}

		if ((Input.GetButton(right)) && canCameraMove(right)) {
			transform.Translate (movementSpeed * Time.deltaTime, 0, 0);
		}

		if ((Input.GetButton(down)) && canCameraMove(down)) {
			transform.Translate (0, 0, -movementSpeed * Time.deltaTime);
		}

		if ((Input.GetButton(left)) && canCameraMove (left)) {
			transform.Translate(-movementSpeed * Time.deltaTime, 0, 0);
		}
	}

	bool canCameraMove (string direction)
	{
		if (direction = forward) {
			if (transform.position.z >= mapSize)
				return false;
			else
				return true;
		}

		else if (direction = right) {
			if (transform.position.x >= mapSize)
				return false;
			else
				return true;
		}

		else if (direction = down) {
			if (transform.position.x <= -mapSize)
				return false;
			else
				return true;
		}

		else (direction = left) {
			if (transform.position.z <= -mapSize)
				return false;
			else
				return true;
		}
	}
}
