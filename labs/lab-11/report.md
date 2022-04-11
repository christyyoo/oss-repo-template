## Checkpoint 1  
![image](https://user-images.githubusercontent.com/60198697/162664971-d40569d2-a92c-4b30-809c-adfbf0aabd46.png)

## Checkpoint 2  
Code:  
```
num_rows = 5
num_cols = 3
num_images = num_rows*num_cols
plt.figure(figsize=(2*2*num_cols, 2*num_rows))
for i in range(num_images):
  plt.subplot(num_rows, 2*num_cols, 2*i+1)
  plot_image(i+9000, predictions[i+9000], test_labels, test_images)
  plt.subplot(num_rows, 2*num_cols, 2*i+2)
  plot_value_array(i+9000, predictions[i+9000], test_labels)
plt.tight_layout()
plt.show()
```  
![image](https://user-images.githubusercontent.com/60198697/162667674-8b776dc9-48eb-4c73-8b2a-f475ede892f0.png)  

## Checkpoint 3  
![converse](https://user-images.githubusercontent.com/60198697/162678682-54b36fde-bbce-45b2-af15-bea747928972.jpg)  
![grey_converse](https://user-images.githubusercontent.com/60198697/162678700-80663734-a7d6-4fa1-ba58-ff2b588aeeb0.jpg)  
![image](https://user-images.githubusercontent.com/60198697/162678775-e20630d1-2e71-448b-a2c7-9eb20e29a497.png)  

![blazer](https://user-images.githubusercontent.com/60198697/162678829-5ce6af9d-e994-452e-9ed0-cbf82b0cb1f6.jpg)  
![grey_blazer](https://user-images.githubusercontent.com/60198697/162678805-100d7c50-4033-4ab9-b57e-e8aab53e397a.jpg)  
![image](https://user-images.githubusercontent.com/60198697/162680308-6f1495bb-8333-4b31-86e2-08a5aab8f122.png)  

![skirt](https://user-images.githubusercontent.com/60198697/162679848-6d6e6945-e619-4846-8672-3db408868f81.jpg)  
![grey_skirt](https://user-images.githubusercontent.com/60198697/162679926-f7d847e9-27b3-4be4-b02d-de4071b6b118.jpg)  
![image](https://user-images.githubusercontent.com/60198697/162680003-d4739ef6-c5a0-43f7-b4b5-eb97239f47a0.png)
