#programming 
Authentication
Client <- Server 
/
{
	"userid" : "UserName"
	"subjects" : \[{subject_title}:"Title", "endpoint":"URL"}, ...\]
}

Client  <- Server  # For professor
GET /SOME_SUBJECT (see endpoint in server response){
	"tests" : \[{
		"test_title" : "String"
		"challenges" : \[{"PROMPT":"question_text", "CORRECT_ANSWER":"answer_text", "IMAGE":"image_url" }, ...]
		}, ...]
}

Client  <- Server  # For student
GET /SOME_SUBJECT (see endpoint in server response){
"tests" : \[{
	"test_title" : "String"
	"challenges" : \[{"PROMPT":"question_text", "IMAGE":"image_url" }, ...]
	}, ...]
}

Client -> Server
POST /SOME_SUBJECT
{
	"test_id":UUID,
	"question_id":UUID,
	"student_answer":"ANSWER"
}

Client <- Server
Response
{
	"test_id":UUID,
	"question_id":UUID,
	"answer_correct":"True|False"
}

Client -> Server
POST /SOME_SUBJECT/result
{
	"test_id":UUID
}

Client -> Server
Desponse
{
	"correct_rate":int,
	...
}