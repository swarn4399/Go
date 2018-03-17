package main

import (
	"net/http"
	"io"
)

func work(w http.ResponseWriter,r *http.Request){
	io.WriteString(w,"Hello I am here")
}
func main(){
	http.HandleFunc("/", work)
	http.ListenAndServe(":8080",nil)
}
