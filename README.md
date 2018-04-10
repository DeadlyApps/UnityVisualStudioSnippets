# Unity Visual Studio Snippets
Convenience Snippets for Unity3d in Visual Studio.

# Installation 
Simply clone repo into your code snippets directory (So you can fork and submit pull requests later :)) :
C:\Users\%USERNAME%\Documents\Visual Studio 2017\Code Snippets\Visual C#\My Code Snippets\

# Usage
Lots of awesome Unity Specific 

"ea+TAB"=>     
```
public event Action EventName = delegate { };
```

"gcic+TAB"=>     
```
var name = GetComponentInChildren<Type>();
```

"gcip+TAB"=>     
```
var name = GetComponentInParent<Type>();
```

"gc+TAB"=>
```
var name = GetComponent<Type>();
```

"rc+TAB"=>
```
[RequireComponent(typeof(Type))]
```

"sf+TAB"=>
```
[SerializeField]
private GameObject Name;
```

"singleton+tab"=>
```
    public static Type Instance { get; set; }

    private void Awake()
    {
        Instance = this;
    }
```

"singletonPlus+TAB"=>
```
    public static Type Instance { get; private set; }

    void Awake()
    {
        if (Instance != null)
        {
            Destroy(gameObject);
        }
        else
        {
            DontDestroyOnLoad(gameObject);
            Instance = this;
        }
    }
```
