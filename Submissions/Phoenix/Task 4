package main

import (
	"net/http"
	"io"
)

func work(w http.ResponseWriter,r *http.Request){
	io.WriteString(w,"<h1>LangChallange</h1><h2>LangChallange</h2><b>LangChallange</b>")
}
func main(){
	http.HandleFunc("/", work)
	http.ListenAndServe(":8080",nil)
}
