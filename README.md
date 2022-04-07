# converstr
func ConvertToString(src string, srcCode string, tagCode string) string {
	srcCoder := mahonia.NewDecoder(srcCode)
	srcResult := srcCoder.ConvertString(src)
	tagCoder := mahonia.NewEncoder(tagCode)
	return tagCoder.ConvertString(srcResult)
}

US-ASCII,ISO-8859-1,Big5,EUC-JP,GB18030,GBK,Shift_JIS,UTF-8,UTF-16,UTF-16BE,UTF-16LE
