---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewOnlineMeeting()
startDateTime , err := time.Parse(time.RFC3339, "2019-07-12T14:30:34.2444915-07:00")
requestBody.SetStartDateTime(&startDateTime) 
endDateTime , err := time.Parse(time.RFC3339, "2019-07-12T15:00:34.2464912-07:00")
requestBody.SetEndDateTime(&endDateTime) 
subject := "User meeting in Microsoft Teams channel."
requestBody.SetSubject(&subject) 
additionalData := map[string]interface{}{
joinMeetingIdSettings := graphmodels.New()
	isPasscodeRequired := false
joinMeetingIdSettings.SetIsPasscodeRequired(&isPasscodeRequired) 
	requestBody.SetJoinMeetingIdSettings(joinMeetingIdSettings)
}
requestBody.SetAdditionalData(additionalData)

result, err := graphClient.Me().OnlineMeetings().Post(context.Background(), requestBody, nil)


```