Its [purpose in life](https://youtu.be/X7HmltUWXgs?t=53s) is to tell you if the
first argument to the script is a valid North Carolina license plate.  It
returns a bool exit status for use in scripting.

It queries the [NCDOT website](https://edmv.ncdot.gov/VehicleRegistration/SpecialPlate/Detail?PlateID=4#term=Standard)
to evaluate if the plate passes their standards checking (not too long, no
invalid characters, etc) and if it is currently available for registration (eg.
not in use on another vehicle).

Usage:
```
  $ ./is-plate-valid root
  No
  $ ./is-plate-valid qwertyui
  Yes
  $
```

It does what it says on the tin.
   --Aaron S. Joyner
