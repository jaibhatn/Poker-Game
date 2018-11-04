# Poker-Game




import java.util.ArrayList;

public class Hand {
	private static final boolean Flush = false;
	private ArrayList<Card> cards = new ArrayList();
	private Object arraylist;

		
	public Hand() {
		
	
	}
	public void arrange() {
		ArrayList<Card>orderedCards= new ArrayList();
		
		for(int z=0; z<5; z++) {
			Card smallCard;
			int smallest=cards.get(0).getNumber();
			smallCard=cards.get(0);
			for(int y=0; y<cards.size(); y++) {
				if(cards.get(y).getNumber()<smallest) {
					smallest=cards.get(y).getNumber();
					smallCard=cards.get(y);
				}
			}
		cards.remove(smallCard);
		orderedCards.add(smallCard);	
			
		}
		cards=orderedCards;
		
		
	}
		
	public String Straight () {
		for (int x=0; x<cards.size(); x++){
		if (cards.get(0).getNumber()+1==cards.get(1).getNumber()) {
			if (cards.get(1).getNumber()+1==cards.get(2).getNumber()) {
				if (cards.get(2).getNumber()+1==cards.get(3).getNumber()) {
					if (cards.get(3).getNumber()+1==cards.get(3).getNumber()) {
						if (cards.get(4).getNumber()+1==cards.get(4).getNumber()) {
							return "Straight";
							
					}
			}
				}
			}
		}
	}
		return null;
	}													
			public boolean Flush() {
			Card flush= cards.get(0);
				String f=cards.get(0).getSuit();
					
				for (int y=0; y<cards.size(); y++) {
						
					}
					return Flush;
				}
				
	

	
	private static int numMatches(String s) {
				// TODO Auto-generated method stub
				return 0;
			}
	public void addCard (Card c) {
		cards.add(c);
	}
	
	public Card showHand () {
		for (int x=0; x<cards.size(); x++) {
			System.out.println(cards.get(x));
			
		}
		return null;
			
	}
		public String checkHand () {
			return null;
			
		}

		
	public int pair() {
		int matches=0;
	
		for (int y=0; y<cards.size(); y++) {
			int n= cards.get(y).getNumber();
			for (int x=y+1; x<cards.size(); x++) {
				
				matches++;
			}
			
		}
			
		return matches;

}			
				
		 public Card getHighestCard() {
			Card highCard= cards.get(0);
			int highest=cards.get(0).getNumber();
			
			for (int y=0; y<cards.size(); y++) {
				
			}
			return highCard;
			
			
	}

		private void get(int i) {
			// TODO Auto-generated method stub
			
		}
	
		


	public String twoPair() {
		for (int x=0; x<5; x++) {
			if (cards.get(0).getNumber()==cards.get(1).getNumber()) {
				if (cards.get(2).getNumber()==cards.get(3).getNumber()) {
					return "Two Pairs";
					for (int y=0; y<5; y++) {
					if (cards.get(1).getNumber()==cards.get(2).getNumber()) {
						if (cards.get(3).getNumber()==cards.get(4).getNumber()) {
							return "Two Pairs";
							for (int z=0; z<5; z++) {
							if (cards.get(0).getNumber()==cards.get(1).getNumber()) {
								if (cards.get(3).getNumber()==cards.get(4).getNumber()) {
									return "Two Pairs";
						}
					}
					
				}
			}
		}
			}
		}
			
		}
	
												
	public String threeofaKind (){
		for (int x=0; x<5; x++) {
			if (cards.get(0).getNumber()==cards.get(1).getNumber()) {
				if (cards.get(1).getNumber()==cards.get(2).getNumber()) {
							return "Three of A Kind";
							
						}
						for (int y=0; y<5; y++) {
							if (cards.get(0).getNumber()==cards.get(3).getNumber()) {
								if (cards.get(3).getNumber()==cards.get(4).getNumber()) {
									return "Three of A Kind";
									
								}
								
								for (int z=0; z<5; z++) {
									if (cards.get(1).getNumber()==cards.get(3).getNumber()) {
										if (cards.get(3).getNumber()==cards.get(4).getNumber()) {
											return "Three of A Kind";	
								}
										for (int t=0; t<5; t++) {
											if (cards.get(2).getNumber()==cards.get(3).getNumber()) {
												if (cards.get(3).getNumber()==cards.get(4).getNumber()) {
													return "Three of A Kind";
						}
							
						}
				}
									}
								}
							}
						}
		}
	
			
		
	
			public String fourofaKind () {
				for (int x=0; x<5; x++) {
					if (cards.get(0).getNumber()==cards.get(1).getNumber()){
						if (cards.get(1).getNumber()==cards.get(2).getNumber()){
								if (cards.get(2).getNumber()==cards.get(3).getNumber()) {
										return "Four of A Kind";
										for (int y=0; y<5; x++) {
											if (cards.get(1).getNumber()==cards.get(2).getNumber()){
												if (cards.get(2).getNumber()==cards.get(3).getNumber()){
														if (cards.get(3).getNumber()==cards.get(4).getNumber()) {
																return "Four of A Kind";
															
						}
							
						}
					}
				}
			
								
								
	public String fullHouse (){
		for (int x=0; x<5; x++){
			if (cards.get(0).getNumber()==cards.get(1).getNumber()){
				if (cards.get(2).getNumber()==cards.get(3).getNumber()) {
					if (cards.get(3).getNumber()==cards.get(4).getNumber()) {
						return "Full House";
						for (int y=0; y<5; y++){
							if (cards.get(0).getNumber()==cards.get(1).getNumber()){
								if (cards.get(2).getNumber()==cards.get(3).getNumber()) {
									if (cards.get(3).getNumber()==cards.get(4).getNumber()) {
										return "Full House";
			}
				
			}
				
			}
						}
					}
				}
	}
					
					public String sFlush () {
						for (int x=0; x<5; x++) {
							if (cards.get(0).getSuit()==cards.get(1).getSuit()) {
								if (cards.get(1).getSuit()==cards.get(2).getSuit()) {
									if (cards.get(2).getSuit()==cards.get(3).getSuit()) {
										if (cards.get(3).getSuit()==cards.get(4).getSuit()) {
									return "Straight Flush";
										}
									}
								}
							}
									
						}
						return null;
							
						}
					
						
					}
				
				

