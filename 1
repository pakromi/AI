import os
import requests
url = "https://vibe.naver.com/track/54692454"  
r = requests.get(url)
r.text

# Okt 형태소 분석기 초기화
okt = Okt()

# 영어 불용어 목록
english_stopwords = [
    "a", "an", "the", "in", "on", "at", "to", "for", "with", "as", "by",
    "I", "you", "he", "she", "it", "we", "they", "my", "your", "his", "her", "its", "our", "their",
    "me", "him", "us", "them", "this", "that", "these", "those",
    "and", "but", "or", "not", "so", "if", "because", "while", "when", "where", "while",
]

# 특수 문자 불용어 목록
special_characters = [
    ".", ",", "!", "?", "-", "_", "(", ")", "[", "]", "{", "}", "'", "\"", ";", ":", "/", "\\",
    # 추가적인 특수 문자를 여기에 추가할 수 있습니다.
]

# 영어 불용어와 특수 문자를 모두 포함하는 불용어 목록 생성
stopwords = english_stopwords + special_characters

# 예시: 불용어 목록을 출력
print(stopwords)

# 가사 파일이 저장된 디렉토리 경로
lyrics_dir = r'C:\Users\Windows(C:)\Windows\21~40.전'

# 결과를 저장할 디렉토리 경로
output_dir = r'C:\Users\Windows(C:)\Windows\21~40.후'

# 결과 디렉토리가 없으면 생성
if not os.path.exists(output_dir):
    os.makedirs(output_dir)

# 가사 파일들의 경로 가져오기
lyrics_files = [os.path.join(lyrics_dir, file) for file in os.listdir(lyrics_dir) if file.endswith('.txt')]

# 각 가사 파일 별로 전처리 수행 및 결과 저장
for file_path in lyrics_files:
    with open(file_path, 'r', encoding='utf-8') as file:
        # 가사 파일 내용 읽기
        song_lyrics = file.read()
        
        # 가사 텍스트 정제 (예: 특수 문자, 숫자 제거)
        song_lyrics = re.sub(r'[^가-힣\s]', '', song_lyrics)
        
        # 형태소 분석 및 토큰화
        tokens = okt.morphs(song_lyrics)
        
        # 불용어 제거
        filtered_tokens = [word for word in tokens if word not in stopwords]
        
        # 결과를 파일로 저장 (다른 폴더에 저장)
        # 파일 이름을 가사 파일 이름과 동일하게 설정
        output_file_path = os.path.join(output_dir, os.path.basename(file_path))
        with open(output_file_path, 'w', encoding='utf-8') as output_file:
            output_file.write(" ".join(filtered_tokens))
