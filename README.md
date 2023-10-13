def create_readme(title, content, items, emphasis, font_size, links):
    readme = ""
    
    readme += f"# {title}\n\n"

    readme += f"**{emphasis}**\n"
    readme += f"<font size={font_size}>{content}</font>\n\n"

    readme += "## 항목\n"
    readme += "<ul>\n"
    for item in items:
        readme += f"  <li>{item}</li>\n"
    readme += "</ul>\n\n"

    readme += f"[더 많은 정보](https://{links})\n"

    with open("README.md", "w") as file:
        file.write(readme)

if __name__ == "__main__":
    title = "Markdown 예제 프로그램"
    content = "이 프로그램은 Markdown 문법을 활용하는 예제입니다."
    items = ["내용 작성", "문서 제목", "항목 열거", "문단 강조", "폰트 크기"]
    emphasis = "Markdown 문법을 활용하여"
    font_size = 4
    links = "www.naver.com"

    create_readme(title, content, items, emphasis, font_size, links)

