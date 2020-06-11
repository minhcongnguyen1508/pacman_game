# pacman_game
Game Pacman Berkeley AI Materials

Complete Reinforcement Learning

# Task 1: Value Iteration trên GridWorld: 10 điểm
 - implement 2 thuật toán:

computeActionFromValues(state): Tìm ra hành động tốt nhất của 1 state

computeQValueFromValues(state, action): Trả về giá trị Qvalue của 1 cặp state action

- test kết quả bằng dòng lệnh:

	python autograder.py -q q1

Sử dụng GUI để test, với các tham số thích hợp:

	python gridworld.py -a value -i 100 -k 10

# Task 2: Q-Learning trên GridWorld (10 điểm)

- cài đặt ở trong qlearningAgents.py  gồm có computeValueFromQValues, getQValue, và computeActionFromQValues.

Lệnh để visualize:

	python gridworld.py -a q -k 5 –m

Lệnh để chạy test:
	
	python autograder.py -q q4
 
# Task 3: Q-Learing trên pacman (20 điểm)
 
Sử dụng qlearningAgents.py  trong bài trên để huấn luyện trên môi trường đơn giản của pacman. Lệnh để test
	
	python pacman.py -p PacmanQAgent -x 2000 -n 2010 -l smallGrid 

Câu lệnh trên có nghĩa: huấn luyện pacman agent với 2000 iterations trên smallGrid

Chú ý: PacmanQAgent được định nghĩa với các giá trị phù hợp hơn cho bài toán pacman. Có thể test lại  bằng cách sử dụng options –a: 

-a epsilon=0.1,alpha=0.3,gamma=0.7

Điểm được chấm theo lệnh: python autograder.py -q q7

Chương trình sẽ train trong 2000 lượt chơi và test trên 100 lượt. Điểm sẽ cho theo số trận thắng trong 100 lượt chơi

# Part 2: 10 Điểm

- Update: Yêu cầu implement thuật toán xấp xỉ Qlearning, điểm đc cho theo score đạt đc khi training với 50 games (10*your_score/MAX_SCORE)

Lệnh test: python autograder.py -q q8
