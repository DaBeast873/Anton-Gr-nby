![1635324755630](https://user-images.githubusercontent.com/35632133/145798951-a256ee3e-2122-421d-9d56-a917c120afc9.jpg)


A unity game programmer who's just graduated game programming at Futuregames Skellefteå.

<h1>STEEZY</h1>

A snowboarding game me and a group of classmates made in ca 1 month that won the competition the school was holding. It also gained some interest from investors stationed in Skellefteå. My role in the project was as a Backend Programmer so I coded all the UI and also started on a leaderboard before the deadline

Below is a function I used to calculate the total time it took the player to finish a track
```
/// <summary>
/// Times and measure the amount of time spent on the level
/// </summary>

private void StopWatchCalculation()
{
    m_AmountOfTime += Time.deltaTime;
    m_Milliseconds = (m_AmountOfTime % 1) * 1000;
    m_Seconds = (int)(m_AmountOfTime  %60);
    m_Minutes = (int)(m_AmountOfTime / 60);      
    
    stopwatchText.text = m_Minutes.ToString("00") + ":" + m_Seconds.ToString("00") + ":" 
    + m_Milliseconds.ToString("000");
}
```

Here's a gameplay trailer of the game

[Trailer](https://user-images.githubusercontent.com/35632133/145810807-31935852-7406-43f0-bcc5-54bafeaeabe6.mp4)


<h1>Wands A Blazing</h1>

A battle royale game that I worked on this fall with another programmer and 3 UX designers.
My role in the project was as a gameplay programmer, so I coded the combat, the UI as well as assisting the backend programmer if needed

An upgrade system I made for the game

``` 
        private void UpdateGun()
        {
            _damage = baseDamage + currentStatModifiers.damageMod;
            _range = baseRange + currentStatModifiers.rangeMod;
            _overheat = baseOverheat + currentStatModifiers.overheatMod;

            _maxAmmo = baseMaxAmmo + currentStatModifiers.maxAmmoMod;
            _currentAmmo = _maxAmmo;
        }      
```

[Trailer](https://youtu.be/vSWZHTEP5Oc)

<h1>Blorb</h1>

I worked on my exam project with some 1st year classmates on a mobile plattformer for Android and IOS where I was the head programmer.
Some gameplay below

![Blorb gameplay](https://user-images.githubusercontent.com/35632133/145793548-617f3b51-28aa-4dc0-a114-c5e690af0d6e.gif)

Below is a coroutine I created that lets the player smoothly switch between 3 different sizes 

```
 private IEnumerator ScaleOverTime(Vector3 toScale)
        {
            if (_isScaling) yield break;

            _isScaling = true;

            float counter = 0;

            Vector3 startSize = transform.localScale;

            while (counter < scaleDuration)
            {
                counter += Time.deltaTime;
                transform.localScale = Vector3.Lerp(startSize, toScale, counter / scaleDuration);
                yield return null;
            }
            _isScaling = false;
        }
```

I'm right now having an internship at Grand Pike AB on their potentially new IP

<h1>Contact me</h1>

If you would like to contact me:

email: antonwg90@gmail.com


phone: (+46)702393292

[Here is my CV if you're interested](https://github.com/DaBeast873/Anton-Granby/files/8958582/CV.Anton.Granby.pdf)
