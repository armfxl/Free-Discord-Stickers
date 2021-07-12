<p align="center">
    <a href="https://discord.gg/VKJeg6nvSH">
  <img src="https://i.imgur.com/1XJhQBe.png"/>
    </a>
</p>

## Free Discord Stickers

I am posting this for educational purposes only. Use this at your own risk as it is against Discord's **[Terms of Service](https://dis.gd/terms)**.  
Please leave a star if you find this useful.   

So, you've probably seen someone using stickers in a Discord chat and you're wondering how to get them? Well, normally you'd have to get Discord Nitro, but in this guide I will show you how to unlock them for free. Thank me later.

### Step 1 | Copy the following code.

```js
const DI = window.DiscordInternals;
const hasLib = !!(DI && DI.versionCompare && DI.versionCompare(DI.version || "", "1.9") >= 0);
    const WebpackModules = hasLib && DI.WebpackModules || (() => {
 
        const req = typeof(webpackJsonp) == "function" ? webpackJsonp([], {
                '__extra_id__': (module, exports, req) => exports.default = req
        }, ['__extra_id__']).default : webpackJsonp.push([[], {
                '__extra_id__': (module, exports, req) => module.exports = req
        }, [['__extra_id__']]]);
        delete req.m['__extra_id__'];
        delete req.c['__extra_id__'];
        const find = (filter, options = {}) => {
            const {cacheOnly = false} = options;
            for (let i in req.c) {
                if (req.c.hasOwnProperty(i)) {
                    let m = req.c[i].exports;
                    if (m && m.__esModule && m.default && filter(m.default))
                        return m.default;
                    if (m && filter(m))
                        return m;
                }
            }
            if (cacheOnly) {
                console.warn('Cannot find loaded module in cache');
                return null;
            }
            console.warn('Cannot find loaded module in cache. Loading all modules may have unexpected side effects');
            for (let i = 0; i < req.m.length; ++i) {
                let m = req(i);
                if (m && m.__esModule && m.default && filter(m.default))
                    return m.default;
                if (m && filter(m))
                    return m;
            }
            console.warn('Cannot find module');
            return null;
        };
        const findByUniqueProperties = (propNames, options) => find(module => propNames.every(prop => module[prop] !== undefined), options);
        const findByDisplayName = (displayName, options) => find(module => module.displayName === displayName, options);
        return {find, findByUniqueProperties, findByDisplayName};
    })();
t = WebpackModules.findByUniqueProperties(["isDeveloper"]);
Object.defineProperty(t,"isDeveloper",{get:_=>1,set:_=>_,configurable:true});
```

### Step 2 | Opening inspect element.

Press `ctrl + shift + i` on your keyboard.

### Step 3 | Drink some water.

You're reading a guide on how to get free Discord stickers, you're probably dehydrated, so drink some water you lazy fuck.

### Step 4 | Paste the code.

Navigate to `console` and paste the code you copied earlier.

### Step 5 | Find experiments in User Settings.

Head over to **User Settings** and look for the following.

![image](https://user-images.githubusercontent.com/55296171/125339686-d75d3c80-e351-11eb-83d9-5dcc27d5845e.png)

### Step 6 | Enable Sticker experiments.

Search for `sticker` and enable `Treatment 1` for all experiments.

![image](https://user-images.githubusercontent.com/55296171/125340203-797d2480-e352-11eb-85ac-ce6b0c3fbee5.png)

### Thanks for reading!   
### By: [armful#0001](https://github.com/armfxl)
