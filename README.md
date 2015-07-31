
# Peanut Labs Reward Center - Publisher Android SDK

Peanut Labs connects your users with thousands of paid online surveys from big brands and market researchers. This SDK allows you to integrate our Reward Center within your Android application. 

#The Reward Center

The Reward Center lists surveys and offers best suited for each of your members. It is highly customizable and positively engaging.

You get paid whenever your members complete a listing, and get to reward them back in the virtual currency of your choice.

All of this and much more is configured  and monitored through our Publisher Dashboard. To learn more and get access to our full set of tools, get in touch with us at publisher.integration@peanutlabs.com

#Integration

Check out <a href="http://peanut-labs.github.io/publisher-doc/" target="_blank">our integration guide</a> for step by step instructions on getting up and running with our Reward Center within your Android application.


#Changelog

v0.2
- Changed "Done" button to "Home" button and replaced into right side
- Replaced "X" button to "Exit" and moved it to the right side
- After done with survey "Done" button led back to the application, changed it into lead back to rewards center
- Supports custom url parameters
- Supports date of birth url parameter
- Supports gender url parameter
- Automatically sets locale for rewards center depends on device locale

*	Open Rewards Center.

``` Java
Open Rewards Center with User Id

PeanutLabsManager pm = PeanutLabsManager.getInstance();
pm.setUserId("EndUserId-AppId-AppKey");
pm.openRewardsCenter(MainActivity.this);

```

* Add dob and gender as a parameter

``` Java
Setting gender // 1(male) or 2(female)
pm.setDob("12-12-1989");

Setting Dob // MM-DD-YYYY
pm.setGender("1");

```

``` Java
First parameter should be var_key and second parameter should be var_val

pm.addCustomParameters("firstName", "bilguun");
pm.addCustomParameters("lastName", "Oyunchimeg");

```
