Unity 每隔一段时间执行操作

```csharp
using UnityEngine;
using System.Collections;

public class KeyAction : MonoBehaviour
{
    public float actionInterval = 1.0f; // 设置操作间隔时间
    private bool isPerformingAction = false; // 用于控制是否正在执行操作

    void Update()
    {
        if (Input.GetKeyDown(KeyCode.Space) && !isPerformingAction)
        {
            isPerformingAction = true;
            StartCoroutine(PerformAction());
        }
        else if (Input.GetKeyUp(KeyCode.Space))
        {
            isPerformingAction = false;
            StopCoroutine(PerformAction());
        }
    }

    IEnumerator PerformAction()
    {
        while (isPerformingAction)
        {
            // 在这里执行你的操作
            Debug.Log("执行操作");
            yield return new WaitForSeconds(actionInterval);
        }
    }
}
```
