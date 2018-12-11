Android Dagger2 Implementation
===========
This repository shows you how to handle Dagger 2 using child fragments.

**Step 1**
Create folder structure as follows

```
   com.projectName/
                  |---->di/
                  |     |
                  |     |---->module/
                  |     |     |
                  |     |     |---->buiders/
                  |     |
                  |     |---->scope/
                  |
                  |---->ui/
```

**Step 2**
Create "App.java" class under the main folder(com.projectName). Extend this class from Application. After that implement onCreate() method. "App.java" shoud look like as follows

``` java
public class App extends Application{
	@Override
	public void onCreate () {
		super.oncreate();
	}
}
```

**Step 3**
In the "AndroidManifest.xml" file, add **android:name=".App"** attribute to Application element.

``` xml
<application
	android:name=".App"
	..................
	..................>
	
	<activity android:name=".ui.MainActivity" />
</application>
```

License
================
	Copyright 2018 Sami Deliceli.

	Licensed under the Apache License, Version 2.0 (the "License");
	you may not use this file except in compliance with the License.
	You may obtain a copy of the License at

		http://www.apache.org/licenses/LICENSE-2.0

	Unless required by applicable law or agreed to in writing, software
	distributed under the License is distributed on an "AS IS" BASIS,
	WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
	See the License for the specific language governing permissions and
	limitations under the License.
