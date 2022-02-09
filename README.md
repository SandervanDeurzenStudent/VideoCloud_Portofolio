# webshop-SvD

<img src ="https://user-images.githubusercontent.com/77112006/142210599-0a4c6a0a-083c-4e63-a0ae-b1153eace27d.png" width=900/>
<img src ="https://user-images.githubusercontent.com/77112006/142210776-e09485b3-8d9e-4566-92b1-2e9d29e1f777.png" width=900/>

### 4. Error handeling
When something unexpected happens, the user should not be left in the dark about this. That's why it's good to put some error handeling in place in case something goes wrong. In the screenshot below, the error that shows when the product service is turned of is shown. This is an error component with some generic text, and then the error below that. In this case, the application failed to fetch, because the product service is turned off.
![image](https://user-images.githubusercontent.com/77112006/150022702-0b9bac5b-60c0-46e3-b19d-a81c7ca09eb1.png)




Sources:
- [CodeSTACKr Auth0 react project](https://github.com/codeSTACKr/react-auth0)

@@ -46,6 +53,13 @@ testing is determining whether the software product meets the expected requireme
<img src ="https://media.discordapp.net/attachments/898556114663252018/910487489083498516/unknown.png?width=1204&height=669" width=900/>
<img src ="https://media.discordapp.net/attachments/898556114663252018/910487588979212338/unknown.png?width=1242&height=670" width=900/>

I also made some front end tests. The first test checks if the Jewellery page doesn't crash. The second one uses mock data to render a single product card, and then checks if this card actually get's rendered. This ensures that when the real data gets fetched, this data also get's rendered. The third test checks for the phrase that's in the ErrorPage component. If it finds it, it means that that component got rendered(this was a work around, I would have liked it better to just check for a component but this works for now, or until someone changes ErrorPage).

![image](https://user-images.githubusercontent.com/77112006/150025935-2c0b2ffa-6582-49b7-aecb-9cc9390114ae.png)



