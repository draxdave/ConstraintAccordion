# ConstraintAccordion 
[![](https://jitpack.io/v/draxdave/ConstraintAccordion.svg)](https://jitpack.io/#draxdave/ConstraintAccordion)


ConstraintAccordion is a [constraint-layout](https://developer.android.com/training/constraint-layout/) based list in Android to display title-description list ex: FAQ , Privacy ,..  . Constraint layout mostly used to implement responsive mobile app layouts. It's also known as a light weight View-Group. 

***

<img src="http://drax.ir/tmp/github/gif/github.com.draxdave.ConstraintAccordion.gif.1.gif" width="250" height="400" />
GIF is loading ...


### Features:
* Super light
* Easy to use



### How to use:

 **Step 1.** Add the **JitPack** repository to your build file.

Add it in your **root build.gradle** at the end of repositories

```
allprojects {

		repositories {

			...

			maven { url 'https://jitpack.io' }

		}

	}
```




**Step 2.** Add the dependency.

```
dependencies {

	        implementation 'com.github.draxdave:ConstraintAccordion:1.0.7'

	}
```




**Step 3.** Push the list.

Place AccordionList tag inside your xml layout or view.
```
...
<ir.drax.constraintaccordionlist.AccordionList
                android:id="@+id/accordion"
                android:layout_width="match_parent"
                android:layout_height="match_parent"/>
...
```



**Step 4.** Push the list.

```
AccordionList accordionList = findViewById(R.id.accordion);
        accordionList
                .setARROW_ICON(R.mipmap.left_arrow_icon)
                .push(accordionItems)
                .build();
```



* You also can push list items asynchronously(one by one or bulk) .

```
accordionList.push(new AccordionItem("Item title" , "Item text content ..."));
```

_That's it!_






### To-do:
* [x] Remove Card-View
* [x] Handle indefinite list items
* [ ] Redesign UI
* [x] Make styles public
* [ ] Display markup
* [ ] Test on old sdk versions





feel free to collaborate/contribute (It would be a pleasure and surely welcomed).




