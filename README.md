A unity game programmer who's right now studying 2nd year of game programming at Futuregames Skellefteå.
[A snowboarding game me and a group of classmates made in ca 1 month](https://www.youtube.com/watch?v=06yZxxC6lMM)
``
private void UpdateGun()
        {
            _damage = baseDamage + currentStatModifiers.damageMod;
            _range = baseRange + currentStatModifiers.rangeMod;
            _overheat = baseOverheat + currentStatModifiers.overheatMod;
            _maxAmmo = baseMaxAmmo + currentStatModifiers.maxAmmoMod;
            _currentAmmo = _maxAmmo;
        }
``
