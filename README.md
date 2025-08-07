# Slovak Keyboard Layout

A Slovak keyboard layout for Linux using X11.

Traditional quote: na Slovensku po Slovensky

<br>

## How To

### Do this step only once

0. Add this entry to the configuration in `/usr/share/X11/xkb/rules/evdev.xml`

   ```
   <layout>
   	<configItem>
   		<name>sk_nsps</name>
   		<shortDescription>sk_nsps</shortDescription>
   		<description>Slovak</description>
   	</configItem>
   	<variantList>
   		<variant>
   			<configItem>
   				<!-- Must match the filename, e.g. sk_nsps -->
   				<name>sk_nsps</name>
   				<description>Slovak (na Slovensku po Slovensky)</description>
   			</configItem>
   		</variant>
   	</variantList>
   </layout>
   ```

### On changes do this

1. Copy the file here from the x11 directory
   - we can use the script `get-keyboard-layout-from-x11-directory.sh`
2. Make some changes to the keyboard layout...
3. Copy the file to the directory
   - we can use the script `put_keyboard_layout_to_x11_directory.sh`
4. Change the keyboard in settings
5. Log out and log in to your account
